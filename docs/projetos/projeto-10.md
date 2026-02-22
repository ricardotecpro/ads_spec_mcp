# Projeto 10 - Web Chat com Ferramentas MCP 🌐

## Objetivo
Criar uma interface web (Frontend) que se conecta a um servidor MCP via SSE, exibindo o feedback visual das ferramentas.

## Requisitos
- HTML/JavaScript básico.
- Servidor MCP rodando com transporte SSE (HTTP).

## Atividades
1. **Conexão SSE**: Implemente o EventSource no JavaScript local para ouvir as mensagens do servidor MCP.
2. **Interface de Log**: Crie uma área na tela que exibe um "spinner" ou mensagem de "Aguardando IA..." sempre que uma requisição `tools/call` estiver em andamento.
3. **Card de Resultado**: Formate o retorno JSON da ferramenta em um card HTML estilizado com CSS.

## Entrega
- Arquivos `index.html` e `style.css`.
- Screenshot do dashboard funcionando e exibindo o resultado de uma ferramenta.

---

> [!IMPORTANT]
> Lembre-se de configurar o CORS no seu servidor backend para permitir a conexão do frontend local.