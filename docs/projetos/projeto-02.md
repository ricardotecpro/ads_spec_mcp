# Projeto 02 - Simulador de Mensagens JSON-RPC 📡

## Objetivo
Explorar a fundo a estrutura das mensagens JSON-RPC 2.0 que viajam via MCP, criando um gerador e validador de mensagens.

## Requisitos
- VS Code.
- Extensão "REST Client" ou Postman.

## Atividades
1. **Modelagem de Requisição**: Escreva um arquivo JSON representando uma requisição de `tools/call` para uma calculadora de IMC.
2. **Criação de Respostas**: Simule as respostas de sucesso (Result) e erro (Error) seguindo o padrão do protocolo.
3. **Validação de Schema**: Utilize uma ferramenta online (JSON Schema Validator) para garantir que sua mensagem segue o contrato definido na documentação do MCP.

## Entrega
- Conjunto de arquivos `.json` com os exemplos de requisição e resposta.
- Breve explicação de cada campo utilizado (jsonrpc, method, id, params).

---

> [!NOTE]
> Lembre-se que o campo `id` deve ser idêntico na requisição e na resposta correspondente.