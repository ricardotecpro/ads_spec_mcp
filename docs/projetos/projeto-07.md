# Projeto 07 - Analista de Dados SQL com IA 📊

## Objetivo
Conectar uma IA a um banco de dados real (SQLite) via MCP, permitindo consultas inteligentes e seguras.

## Requisitos
- Biblioteca `sqlite3` ou similar.
- Banco de dados `clientes.db` de exemplo.

## Atividades
1. **Ferramenta de Busca**: Crie a Tool `query_database` que aceita parâmetros de busca (ex: nome do cliente).
2. **Segurança**: Implemente queries parametrizadas para evitar SQL Injection.
3. **Recurso de Schema**: Crie um Resource `mcp://db/schema` que retorna a lista de tabelas e colunas para a IA se orientar.
4. **Desafio**: Peça para a IA: "Quais clientes compraram mais de R$ 500,00 este mês?".

## Entrega
- Código do servidor.
- Arquivo `.db` utilizado.
- Relatório de como você protegeu o banco contra deleções acidentais.

---

> [!CAUTION]
> Dê permissão apenas de LEITURA (SELECT) para o usuário do banco utilizado pelo MCP.