# Exercícios: Aula 08 - Segurança no MCP 🔐

### 🟢 Nível Básico

1.  O que é **Sandboxing** e por que ele é recomendado para servidores MCP?
2.  Explique o risco de uma IA ter acesso total ao seu sistema de arquivos (`C:\` ou `/`).

### 🟡 Nível Intermediário

3.  Diferencie **Autenticação** de **Auditoria** no contexto de um servidor MCP corporativo.
4.  Como você evitaria que um usuário desse comandos maliciosos para a IA que resultassem em exclusão de dados via MCP? (Cite a técnica de "Aprovação Humana").

### 🔴 Nível Desafio

5.  **Análise de Risco**: Um servidor MCP expõe uma ferramenta de execução de códigos Python (`exec()`).
    *   Liste 3 perigos deste cenário.
    *   Proponha 2 medidas de mitigação (ex: Docker, limite de tempo) para tornar este servidor minimamente seguro.