# Projeto 05 - Monitor de Conexão e Logs (Sampling) 🔄

## Objetivo
Implementar o recurso de Sampling, onde o servidor solicita uma ação inteligente da IA para processar logs técnicos.

## Requisitos
- SDK MCP instalado.
- Servidor rodando em modo Stdio.

## Atividades
1. **Geração de Logs**: Crie uma função que gera logs de erro aleatórios no seu servidor.
2. **Pedido de Sampling**: Quando um erro crítico ocorrer, o servidor deve enviar uma requisição `mcp/sampling` ao cliente, pedindo para a IA resumir o erro e sugerir uma solução.
3. **Log de Feedback**: Exiba no terminal a sugestão enviada pela IA.

## Entrega
- Código-fonte demonstrando o uso do método `sampling` do SDK.
- Log de execução mostrando a pergunta do servidor e a resposta da IA.

---

> [!IMPORTANT]
> O Servidor não tem inteligência própria. Ele depende do Cliente (Claude/IDE) para processar o prompt de sampling.