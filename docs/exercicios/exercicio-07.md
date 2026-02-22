# Exercícios: Aula 07 - Integração com Banco de Dados 💾

### 🟢 Nível Básico

1.  Por que devemos usar **Resources** para exibir relatórios e **Tools** para fazer buscas filtradas?
2.  O que significa "parametrização de queries" em bancos de dados?

### 🟡 Nível Intermediário

3.  Como os comentários no esquema (Schema documentation) ajudam a IA a realizar consultas mais precisas?
4.  Explique o risco de dar permissão de `DROP TABLE` para um servidor MCP que será usado por um Chatbot público.

### 🔴 Nível Desafio

5.  **Cenário de Implementação**: Você precisa expor uma tabela de `Vendas`.
    *   Crie uma Tool chamada `get_sales_by_period` que aceita `start_date` e `end_date`.
    *   Escreva a query SQL (ou o comando do seu banco preferido) utilizando parâmetros seguros para evitar injeção.