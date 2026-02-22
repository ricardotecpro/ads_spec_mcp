# Projeto 11 - Cluster de Microsserviços MCP 🔌

## Objetivo
Simular uma arquitetura distribuída onde um único Cliente MCP orquestra chamadas para três servidores diferentes.

## Requisitos
- 3 pequenos servidores MCP rodando em portas ou processos diferentes.

## Atividades
1. **Configuração Multi-Server**: No seu Cliente (Claude/Cursor), registre os três servidores simultaneamente.
    - Servidor A: Consulta Preços.
    - Servidor B: Consulta Estoque.
    - Servidor C: Envia Notificações.
2. **Orquestração**: Faça uma pergunta que exija dados dos três servidores (ex: "Verifique se o Item X está em estoque, qual o preço e me avise por e-mail").
3. **Análise de Conflitos**: Verifique se a IA consegue lidar com ferramentas de nomes similares em servidores diferentes.

## Entrega
- Arquivo de configuração do cliente usado.
- Log da conversa onde a IA utiliza os três servidores para resolver um único problema.

---

> [!NOTE]
> Este projeto demonstra o verdadeiro poder da "interoperabilidade" do MCP.