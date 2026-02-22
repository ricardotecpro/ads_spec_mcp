# Aula 15 - Projeto Prático Orientado 🎓

!!! tip "Objetivo"
    **Objetivo**: Consolidar todo o conhecimento adquirido ao longo do curso através do desenvolvimento de um sistema real utilizando o protocolo MCP. Vamos construir um **Assistente de Pesquisa Acadêmica**.

---

## 1. Visão Geral do Projeto: Assistente Acadêmico 📚

O objetivo é criar um assistente que ajude estudantes a organizar suas referências bibliográficas, pesquisar em bancos de artigos (simulados) e gerar resumos padronizados.

### Componentes do Projeto:
*   **Servidor MCP**: Desenvolvido em Node.js ou Python.
*   **Base de Dados**: Arquivos Markdown ou Banco SQLite contendo resumos de artigos.
*   **Integração**: Conexão com o Claude Desktop ou uma IDE compatível.

---

## 2. Requisitos Técnicos 🏗️

O seu servidor deve obrigatoriamente implementar:

1.  **Resources**:
    *   `mcp://biblioteca/lista-artigos`: Lista de todos os títulos e autores.
    *   `mcp://biblioteca/artigo/[id]`: Conteúdo completo de um artigo específico.
2.  **Tools**:
    *   `search_articles(query: string)`: Busca artigos por palavras-chave.
    *   `export_bibtex(article_id: string)`: Gera a referência no formato BibTeX.
3.  **Prompt**:
    *   `generate-literature-review`: Um template especializado em análise crítica de textos acadêmicos.

---

## 3. Passo a Passo da Implementação 🛠️

### Passo 1: Configuração do Ambiente
Inicie o projeto, instale o SDK e as dependências de banco de dados.

### Passo 2: Implementação dos Resources
Crie a lógica para ler os arquivos de artigos da sua pasta `data/`.

### Passo 3: Implementação das Tools
Codifique a lógica de busca (pode usar um simples `grep` ou busca SQL).

### Passo 4: Registro e Teste
Registre tudo no servidor e use o **Inspector** para validar cada funcionalidade.

---

## 4. Documentação Técnica 📄

Um projeto real precisa de uma boa documentação. Crie um `README.md` para o seu servidor contendo:
*   Instruções de instalação.
*   Lista de ferramentas disponíveis com exemplos de chamada.
*   Variáveis de ambiente necessárias (ex: `DB_PATH`).

---

## 5. Prática: Validando o Fluxo Completo 💻

Abra o Claude Desktop e faça o seguinte teste:

```termynal
Usuário: "Quais artigos você tem sobre Machine Learning?"
IA: (Chama search_articles...) "Tenho 2 artigos..."
Usuário: "Resuma o primeiro e me dê a referência BibTeX."
IA: (Lê o Resource e chama export_bibtex...) [RESULTADO COMPLETO]
```

---

## 6. Mini-Projeto: Extensão do Assistente 🧪

Adicione uma nova Tool ao seu projeto:
*   `add_note(article_id: string, note: string)`: Permite que a IA salve anotações do usuário sobre um artigo específico em um arquivo `notes.txt`.

---

## 7. Exercícios de Fixação 📝

1.  Por que é importante testar as Tools individualmente antes de conectar ao Claude?
2.  Como o uso de **Templates de Prompts** pode ajudar um estudante a escrever melhor suas monografias?
3.  O que você faria para garantir que o seu assistente não "inventasse" artigos que não existem na sua biblioteca?

---

!!! info "Dica"
    Este projeto é excelente para seu portfólio! Hospede o código no GitHub e inclua um vídeo demonstrativo da IA usando suas ferramentas.

**Próxima Aula**: [Tendências e Futuro do MCP](./aula-16.md) ✨