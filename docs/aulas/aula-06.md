# Aula 06 - Implementação de um Servidor MCP (Backend) ⚙️

!!! tip "Objetivo"
    **Objetivo**: Aprender a estruturar um projeto de servidor MCP do zero, utilizando SDKs oficiais (Node.js ou Python) e registrando funcionalidades reais.

---

## 1. Escolhendo sua Stack 🛠️

O MCP possui SDKs robustos para as duas linguagens mais populares em IA:

*   **Node.js / TypeScript**: Ideal para alta performance e ecossistema web.
*   **Python**: Perfeito para ciência de dados, machine learning e automação de scripts.

---

## 2. Estrutura de Projeto (Node.js) 📂

Um servidor MCP bem organizado segue este padrão:

```termynal
$ npm init -y
$ npm install @modelcontextprotocol/sdk
$ ls
├── src/
│   ├── index.ts      # Ponto de entrada
│   ├── tools.ts      # Definição de ferramentas
│   └── resources.ts  # Definição de recursos
├── package.json
└── tsconfig.json
```

---

## 3. Registrando uma Ferramenta (Tool) 🛠️

No código, definimos o esquema da ferramenta e a lógica de execução.

```typescript
// Exemplo em TypeScript
server.tool(
  "calculate_area",
  "Calcula a área de um retângulo",
  {
    width: z.number().describe("Largura do retângulo"),
    height: z.number().describe("Altura do retângulo"),
  },
  async ({ width, height }) => {
    return {
      content: [{ type: "text", text: `A área é ${width * height}` }],
    };
  }
);
```

---

## 4. O Servidor em Ação (Python) 🐍

Python utiliza decoradores para simplificar o registro:

```python
from mcp.server.fastmcp import FastMCP

mcp = FastMCP("MeuServidor")

@mcp.tool()
def somar_numeros(a: int, b: int) -> int:
    """Soma dois números inteiros."""
    return a + b
```

---

## 5. Testes Locais e Depuração 🧪

Antes de conectar ao Claude ou outra IDE, testamos via terminal usando o `mcp-inspector`.

```termynal
$ npx @modelcontextprotocol/inspector node build/index.js
[INFO] Inspetor iniciado na porta 3000
[SUCCESS] Servidor conectado!
[ACTION] Tente chamar 'somar_numeros' com argumentos {a: 5, b: 10}
```

---

## 6. Mini-Projeto: Ola Mundo MCP 🚀

1.  Crie uma pasta para seu projeto.
2.  Configure o SDK (Node ou Python).
3.  Implemente uma Tool chamada `get_current_time` que retorna a hora atual do sistema.
4.  Valide o funcionamento no Inspetor.

---

## 7. Exercícios de Fixação 📝

1.  Para que serve o objeto `z` (Zod) no exemplo de TypeScript?
2.  Qual a vantagem de usar o `FastMCP` em Python para prototipagem rápida?
3.  O que acontece se o seu servidor não exportar nenhuma Tool ou Resource?

---

!!! concept "Aviso"
    Lembre-se: em Stdio, o seu servidor escreve logs em `stderr`. Nunca use `console.log` para mensagens de debug, pois isso quebrará o protocolo JSON-RPC que usa o `stdout`.

**Próxima Aula**: [Integração do MCP com Banco de Dados](./aula-07.md) 💾
