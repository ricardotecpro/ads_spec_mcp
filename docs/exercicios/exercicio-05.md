# Exercícios: Aula 05 - Comunicação C/S 🔄

### 🟢 Nível Básico

1.  Qual a principal diferença entre uma requisição (Request) e uma notificação (Notification)?
2.  O que é o `id` em uma mensagem JSON-RPC e por que ele é incremental?

### 🟡 Nível Intermediário

3.  Explique o que acontece durante o **Handshake** inicial entre o cliente e o servidor.
4.  Se o servidor retornar o código de erro `-32601` (Method not found), o que provavelmente está errado na chamada do cliente?

### 🔴 Nível Desafio

5.  **Análise de Fluxo**: Desenhe a sequência de mensagens JSON-RPC para o seguinte cenário:
    *   O Cliente pede a lista de recursos.
    *   O Servidor responde com dois recursos (logs e docs).
    *   O Cliente lê o recurso de logs.
    *   O Servidor retorna o conteúdo do log.