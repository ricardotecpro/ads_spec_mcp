# Projeto 13 - Suíte de Testes Automatizados 🧪

## Objetivo
Implementar uma suíte de testes robusta para um servidor MCP, cobrindo lógica de negócio e conformidade com o protocolo.

## Requisitos
- Jest ou Vitest (Node) / PyTest (Python).

## Atividades
1. **Testes Unitários**: Escreva testes para as funções internas das suas ferramentas, garantindo que elas lidam com inputs válidos e inválidos.
2. **Teste de Integração**: Utilize o SDK em modo de teste para simular o Handshake inicial e verificar se o servidor retorna as `capabilities` corretas.
3. **Teste de Erro**: Provoque um erro de `Invalid Params` e verifique se o código de erro JSON-RPC retornado é o `-32602`.

## Entrega
- Pasta `tests/` com os arquivos de teste.
- Relatório de cobertura (coverage report).

---

> [!NOTE]
> Testar um servidor MCP exige garantir que o JSON gerado é válido, não apenas que a função rodou.