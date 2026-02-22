# Projeto 08 - Firewall de Prompt e Auditoria 🔐

## Objetivo
Implementar camadas de segurança em um servidor MCP para validar entradas e registrar ações críticas.

## Requisitos
- Servidor MCP funcional anterior.

## Atividades
1. **Validação de Input**: Crie uma função que bloqueia palavras-chave perigosas nos argumentos das tools (ex: "DROP", "DELETE", "../").
2. **Log de Auditoria**: Implemente um sistema que grava em um arquivo `audit.log` todas as chamadas de ferramentas, incluindo o timestamp e os parâmetros recebidos.
3. **HITL (Human-In-The-Loop)**: Simule uma ferramenta de `deletar_usuario` que retorna uma mensagem pedindo confirmação manual via interface do cliente.

## Entrega
- Código com as travas de segurança.
- Exemplo do arquivo `audit.log`.

---

> [!NOTE]
> Segurança não é apenas código, é estratégia. Pense em como um usuário mal-intencionado tentaria burlar seu servidor.