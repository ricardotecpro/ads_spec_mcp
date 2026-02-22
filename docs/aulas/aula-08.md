# Aula 08 - Segurança no MCP 🔐

!!! tip "Objetivo"
    **Objetivo**: Compreender os riscos de segurança inerentes à conexão de IAs com sistemas externos e implementar camadas de proteção, autenticação e controle de acesso em servidores MCP.

---

## 1. O Modelo de Ameaças 🛡️

Ao expor ferramentas para uma IA, abrimos portas para possíveis ataques ou erros catastróficos.

*   **Execução Remota de Código (RCE)**: Uma Tool que permite rodar comandos shell sem filtro.
*   **Vazamento de Dados (PII)**: IA lendo dados sensíveis de usuários sem autorização.
*   **Prompt Injection**: O usuário engana a IA para que ela execute ações maliciosas via MCP.

---

## 2. Autenticação e Autorização 🔑

O MCP não impõe um método único, mas recomenda padrões:

*   **API Keys**: Chaves simples para acesso direto entre Cliente e Servidor.
*   **OAuth2**: Para integrações que exigem permissão explícita do usuário (ex: acessar Google Drive).
*   **Local Trust**: Em conexões Stdio, a confiança é baseada no fato de o servidor rodar na mesma máquina que o cliente.

---

## 3. Sandboxing e Isolamento 🏗️

Sempre assuma que o código que o servidor executa pode ser perigoso.

*   **Docker**: Rode seu servidor MCP dentro de um container isolado.
*   **Limitação de Recursos**: Restrinja memória e CPU para evitar ataques de negação de serviço (DoS).
*   **Acesso ao Sistema de Arquivos**: Use caminhos absolutos e valide se a IA não está tentando acessar pastas fora do diretório permitido (`../`).

---

## 4. Auditoria e Logging 📜

"Quem fez o quê, quando e como?". Manter logs é essencial para conformidade e segurança.

!!! concept "Auditoria no MCP"
    Sempre registre:
    1.  O ID da sessão do usuário.
    2.  O nome da ferramenta chamada.
    3.  Os argumentos passados.
    4.  O resultado retornado.

---

## 5. Prática: Validando Argumentos Sensíveis 💻

Vamos criar um middleware simples de validação de segurança.

```typescript
// Exemplo de validação de diretório
function safePath(targetPath: string) {
    const root = "/app/data";
    const resolvedPath = path.resolve(root, targetPath);
    if (!resolvedPath.startsWith(root)) {
        throw new Error("Acesso negado: Tentativa de Path Traversal!");
    }
    return resolvedPath;
}
```

---

## 6. Mini-Projeto: Checklist de Segurança 🧪

Crie um documento de "Políticas de Segurança" para um servidor MCP que acessa dados de RH.

1.  Defina quais colunas são estritamente proibidas (ex: senhas, hashes).
2.  Estabeleça um limite de requisições por minuto (Rate Limit).
3.  Crie uma regra para quando a IA pedir para deletar um usuário (ex: Exigir aprovação manual via Cliente).

---

## 7. Exercícios de Fixação 📝

1.  O que é **Prompt Injection** e como ele pode afetar uma Tool do MCP?
2.  Por que o isolamento via Docker é uma boa prática para servidores MCP?
3.  Qual a diferença entre Autenticação e Auditoria?

---

!!! warning "Importante"
    A segurança no MCP é uma responsabilidade compartilhada entre o desenvolvedor do servidor e o desenvolvedor do cliente. Nunca confie cegamente nos inputs que vêm do Modelo de IA.

**Próxima Aula**: [MCP e Engenharia de Prompt](./aula-09.md) 🧠
