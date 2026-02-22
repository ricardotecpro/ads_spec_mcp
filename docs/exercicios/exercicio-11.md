# Exercícios: Aula 11 - MCP e Microsserviços 🔌

### 🟢 Nível Básico

1.  O que é um **Orquestrador MCP**?
2.  Explique o conceito de **Desacoplamento** ao usar múltiplos servidores MCP pequenos.

### 🟡 Nível Intermediário

3.  Por que o **Lazy Loading** de servidores MCP é importante para a performance do sistema do usuário?
4.  Como você usaria um **Correlation ID** para debugar uma falha que aconteceu em um fluxo envolvendo três microsserviços diferentes?

### 🔴 Nível Desafio

5.  **Design de Arquitetura**: Desenhe (ou descreva) o fluxo técnico de um assistente de IA que precisa:
    *   Buscar o preço de um produto (Servidor de Catálogo).
    *   Verificar o estoque para o CEP do usuário (Servidor de Logística).
    *   Gerar um link de pagamento (Servidor Financeiro).
    *   *Desafio*: O que a IA deve responder se o Servidor de Logística estiver offline?