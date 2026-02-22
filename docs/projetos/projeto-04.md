# Projeto 04 - Catálogo de Recursos Dinâmicos 📂

## Objetivo
Implementar um servidor MCP que expõe arquivos locais como Resources e ferramentas de edição como Tools.

## Requisitos
- Node.js ou Python.
- Pasta com arquivos `.txt` de exemplo.

## Atividades
1. **Exposição de Resources**: Registre um recurso dinâmico que lista todos os arquivos de uma pasta específica.
2. **Leitura de Conteúdo**: Implemente a lógica para que a IA consiga ler o conteúdo de um arquivo selecionado via URI `mcp://local/file/nome.txt`.
3. **Tool de Escrita**: Crie uma ferramenta `write_to_file` que permite à IA salvar novos textos na pasta.

## Entrega
- Código do servidor com `resources/list`, `resources/read` e `tools/call`.
- Documentação das URIs utilizadas.

---

> [!WARNING]
> Tenha cuidado com a segurança de caminhos (Path Traversal). Garanta que a IA só acesse a pasta de projeto definida.