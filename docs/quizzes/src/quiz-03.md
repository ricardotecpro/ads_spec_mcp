# Quiz 03 - Arquitetura do MCP 🏗️

1. Quais são as três entidades principais em uma arquitetura MCP?
    - [ ] Usuário, Monitor e Teclado.
    - [ ] Database, API e Frontend.
    - [x] Modelo (LLM), Cliente (Host) e Servidor (Source).
    - [ ] Python, Node e Java.
    *Explicação: Estes três componentes formam o triângulo de comunicação do MCP.*

2. O que é o "Handshake" na inicialização de um servidor MCP?
    - [ ] Um comando para desligar o servidor.
    - [x] Um processo de troca de informações iniciais e capacidades.
    - [ ] Uma forma de criptografar o disco rígido.
    - [ ] Um aperto de mão físico entre os desenvolvedores.
    *Explicação: No handshake, o cliente e o servidor concordam sobre versões e funcionalidades.*

3. No transporte "Stdio", como as mensagens são enviadas?
    - [ ] Por ondas de rádio.
    - [ ] Via cabos de fibra ótica exclusivos.
    - [x] Através da Entrada e Saída Padrão (terminal) do sistema.
    - [ ] Por sinal de fumaça digital.
    *Explicação: Stdio usa o canal de comunicação de processos do sistema operacional.*

4. Qual a função do "MCP Client" (ex: Claude Desktop)?
    - [ ] Treinar a inteligência artificial.
    - [x] Orquestrar a conexão entre a inteligência (Modelo) e os dados (Servidores).
    - [ ] Servir como banco de dados principal.
    - [ ] Criar códigos de programação sozinho.
    *Explicação: O cliente é o "hospedeiro" que gerencia as permissões e o tráfego.*

5. Por que o Servidor MCP nunca conversa diretamente com o Modelo (LLM)?
    - [ ] Por falta de compatibilidade técnica.
    - [x] Por questões de segurança e controle centralizado no Cliente.
    - [ ] Porque o Modelo não tem internet.
    - [ ] Porque o Servidor é muito lento.
    *Explicação: O Cliente atua como um filtro de segurança e gerenciador de estado.*

6. O que o transporte "HTTP with SSE" permite que o Stdio não permite?
    - [ ] Mais velocidade de processamento.
    - [x] Conexão entre computadores diferentes através da rede/internet.
    - [ ] Uso exclusivo de Python.
    - [ ] Melhor design de interface.
    *Explicação: SSE (Server-Sent Events) sobre HTTP permite arquiteturas distribuídas remotamente.*

7. Durante o Handshake, o que é o campo "capabilities"?
    - [ ] O limite de memória do servidor.
    - [x] A lista de funcionalidades (Tools, Resources, Prompts) que o servidor oferece.
    - [ ] O nome do criador do servidor.
    - [ ] A velocidade da conexão Wi-Fi.
    *Explicação: As capacidades definem o "cardápio" de opções que o servidor disponibiliza.*

8. Qual o estado final de um ciclo de vida de conexão MCP bem-sucedido?
    - [ ] crashed
    - [ ] pending
    - [x] shutdown (Encerramento limpo)
    - [ ] infinite_loop
    *Explicação: Uma boa aplicação encerra seus processos de forma controlada.*

9. Se um servidor é iniciado via "Stdio", como ele é executado pelo Cliente?
    - [ ] Como uma página web no navegador.
    - [x] Como um processo filho (subprocess) do próprio Cliente.
    - [ ] Como um plugin do Microsoft Excel.
    - [ ] Como um driver de impressora.
    *Explicação: O Cliente lança o executável do servidor e captura seu fluxo de dados.*

10. Qual a vantagem do transporte Stdio em termos de segurança?
    - [ ] Nenhuma, é o mais inseguro.
    - [ ] É criptografado por satélite.
    - [x] Os dados nunca saem da máquina local do usuário.
    - [ ] Não exige o uso de senhas.
    *Explicação: Por ser local, não há risco de interceptação de dados por hackers na rede externa.*
