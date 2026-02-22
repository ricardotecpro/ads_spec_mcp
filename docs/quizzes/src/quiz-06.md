# Quiz 06 - Implementação de Servidor MCP ⚙️

1. Qual a função principal do SDK oficial do MCP?
    - [ ] Criar a interface visual da IA.
    - [x] Facilitar o registro de ferramentas e a gestão da comunicação JSON-RPC.
    - [ ] Melhorar a velocidade da CPU.
    - [ ] Traduzir o código TypeScript para Python automaticamente.
    *Explicação: O SDK abstrai as complexidades do protocolo para o desenvolvedor.*

2. Em TypeScript, para que serve a biblioteca "Zod" no servidor MCP?
    - [ ] Para estilizar o terminal.
    - [x] Para validar os tipos de dados dos argumentos enviados pela IA.
    - [ ] Para conectar ao banco de dados SQL.
    - [ ] Para comprimir os arquivos do projeto.
    *Explicação: Zod garante que, se a IA enviar um texto onde deveria ser um número, o erro seja detectado.*

3. No Python, qual biblioteca facilita a criação rápida de servidores MCP?
    - [ ] Django
    - [ ] Pandas
    - [x] FastMCP
    - [ ] PyTorch
    *Explicação: FastMCP é um wrapper que simplifica drasticamente o registro de tools em Python.*

4. Ao implementar uma Tool, o que o campo `.describe()` faz?
    - [ ] Muda a cor do código.
    - [x] Fornece informações vitais para o LLM entender para que serve aquele parâmetro.
    - [ ] Escreve um comentário no arquivo `README.md`.
    - [ ] Define o tamanho máximo do arquivo.
    *Explicação: É "Engenharia de Prompt" dentro do código para guiar a inteligência da IA.*

5. Qual o comando usado para testar um servidor MCP local sem precisar do Claude Desktop?
    - [ ] `node run server`
    - [ ] `python main.py`
    - [x] `npx @modelcontextprotocol/inspector`
    - [ ] `mcp-start`
    *Explicação: O Inspector é a ferramenta oficial de depuração e testes do MCP.*

6. O que representa o valor de retorno de uma Tool no código?
    - [ ] O nome do servidor.
    - [x] O conteúdo (texto, imagem, etc.) que será enviado de volta para a IA.
    - [ ] Um comando de encerramento do sistema.
    - [ ] A data e hora da execução.
    *Explicação: O retorno é o "resultado" que a IA usará para gerar sua resposta final.*

7. Por que devemos compilar o código TypeScript (usando `tsc`) antes de rodar o servidor no MCP?
    - [ ] Porque o protocolo MCP não gosta de arquivos `.ts`.
    - [x] Porque o ambiente de execução (Node.js) executa código JavaScript (`.js`), não TypeScript diretamente.
    - [ ] Para economizar espaço em disco.
    - [ ] É um requisito apenas para servidores Python.
    *Explicação: O processo de build transforma o código tipado em código executável pelo Node.*

8. O que acontece se duas Tools forem registradas com o mesmo nome em um servidor?
    - [ ] A IA escolhe a melhor.
    - [ ] O servidor ignora o erro.
    - [x] O servidor geralmente gerará um erro de conflito durante a inicialização.
    - [ ] Elas se fundem em uma ferramenta só.
    *Explicação: Cada nome de ferramenta deve ser único dentro de um mesmo servidor.*

9. Qual a utilidade do arquivo `package.json` em um projeto de servidor MCP em Node.js?
    - [ ] Guardar as fotos do projeto.
    - [x] Gerenciar dependências e scripts de automação do projeto.
    - [ ] Configurar o papel de parede do terminal.
    - [ ] Armazenar o cache do banco de dados.
    *Explicação: É o coração do gerenciamento de projetos Node, listando o SDK e scripts de build.*

10. No desenvolvimento de um servidor MCP, o que significa "Logging via Stderr"?
    - [ ] Salvar logs em um banco de dados remoto.
    - [x] Imprimir mensagens de debug em um canal que o Cliente MCP capture sem confundir com dados JSON-RPC.
    - [ ] Esconder erros do usuário.
    - [ ] Traduzir erros para o inglês automaticamente.
    *Explicação: Logs em `stderr` aparecem nos consoles de monitoramento do cliente (ex: Claude logs).*
