# Quiz 05 - Comunicação Cliente ↔ Servidor 🔄

1. Qual a diferença fundamental entre uma "Request" e uma "Notification" no JSON-RPC?
    - [ ] Requests são em inglês, Notifications em português.
    - [x] Requests esperam uma resposta do receptor; Notifications são informativas e não esperam resposta.
    - [ ] Notifications são apenas para erros.
    - [ ] Requests não possuem ID.
    *Explicação: No protocolo, o receptor deve responder a uma Request citando o seu ID.*

2. Por que o campo `id` é obrigatório em uma Request?
    - [ ] Para contar quantos usuários o sistema tem.
    - [x] Para que o cliente consiga relacionar a resposta recebida à pergunta original.
    - [ ] Para identificar o nome do programador.
    - [ ] Para criptografar a mensagem.
    *Explicação: Como as mensagens podem chegar fora de ordem, o ID vincula pergunta e resposta.*

3. O que acontece se o servidor retornar um erro com o código `-32601`?
    - [ ] O banco de dados caiu.
    - [x] O método (tool/resource) solicitado pelo cliente não existe no servidor.
    - [ ] A internet está lenta.
    - [ ] O JSON está mal escrito.
    *Explicação: Este é o código padrão para "Method not found" (Método não encontrado).*

4. O recurso de "Sampling" permite que:
    - [ ] O servidor colete amostras de sangue do usuário.
    - [x] O servidor solicite ao modelo de IA (via cliente) que gere uma resposta ou complete um texto.
    - [ ] O cliente tire uma foto do servidor.
    - [ ] A IA seja treinada com novos dados.
    *Explicação: No sampling, a lógica de execução "pede ajuda" para a inteligência da IA.*

5. O que são "Server-Sent Events" (SSE) no contexto do transporte HTTP?
    - [ ] E-mails enviados pelo servidor.
    - [x] Uma conexão unidirecional onde o servidor envia atualizações constantes para o cliente.
    - [ ] Mensagens de erro que aparecem no terminal.
    - [ ] Eventos de marketing da Anthropic.
    *Explicação: SSE é usado para manter o cliente atualizado sobre o estado do servidor remoto.*

6. Qual o objetivo do comando `notifications/initialized` enviado pelo Cliente?
    - [ ] Desligar o servidor.
    - [x] Confirmar que o cliente recebeu as capacidades e que a conexão está pronta para uso.
    - [ ] Enviar a senha do administrador.
    - [ ] Pedir a lista de ferramentas novamente.
    *Explicação: É a etapa final do Handshake, concluindo a fase de configuração.*

7. No tráfego de mensagens, onde os erros do servidor MCP (em Stdio) devem ser registrados para não quebrar a comunicação?
    - [ ] No `stdout`.
    - [ ] No banco de dados.
    - [x] No `stderr` (Saída de erro padrão).
    - [ ] Em um arquivo `.txt` na área de trabalho.
    *Explicação: O `stdout` é reservado para mensagens JSON-RPC puras; logs vão para o `stderr`.*

8. O que é um "Timeout de Request" no MCP?
    - [ ] Quando o computador desliga por falta de bateria.
    - [x] Quando o servidor demora mais do que o esperado para responder a uma Request do cliente.
    - [ ] Quando o usuário para de digitar.
    - [ ] Quando a sessão expira após 10 minutos.
    *Explicação: O cliente desiste de esperar a resposta para evitar travamentos infinitos.*

9. Qual o papel do receptor (servidor ou cliente) ao receber uma Notificação?
    - [ ] Deve enviar um OK imediatamente.
    - [x] Deve apenas processar a informação internamente, sem enviar resposta.
    - [ ] Deve reiniciar o serviço.
    - [ ] Deve registrar um erro se não houver ID.
    *Explicação: Notificações seguem o padrão "fire and forget" (dispare e esqueça).*

10. Se a IA sugerir o uso de uma ferramenta, quem envia a `Request` de fato para o servidor?
    - [ ] A IA diretamente.
    - [ ] O usuário final.
    - [x] O MCP Client (ex: Claude Desktop).
    - [ ] O Sistema Operacional.
    *Explicação: O Cliente atua como o braço executor que traduz o desejo da IA em uma chamada técnica.*