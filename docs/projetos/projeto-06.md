# Projeto 06 - Servidor MCP "Gerenciador de Tarefas" 📝

## Objetivo
Construir um servidor MCP funcional completo que permita à IA gerenciar uma lista de tarefas (Todo List) em memória.

## Requisitos
- Node.js (TypeScript) ou Python (FastMCP).

## Atividades
1. **Definição de Tools**: Crie ferramentas para:
    - `add_task(titulo, prioridade)`
    - `list_tasks()`
    - `complete_task(id)`
2. **Validação com Zod**: Garanta que as prioridades sejam apenas "Alta", "Média" ou "Baixa".
3. **Teste no Claude Desktop**: Adicione seu servidor ao arquivo de configuração e peça à IA para: "Crie uma lista de tarefas para meu dia de hoje".

## Entrega
- Código do servidor.
- Vídeo ou prints da IA interagindo com as tarefas (adicionando, listando e concluindo).

---

> [!TIP]
> Use um array simples em memória para armazenar as tarefas durante a sessão.