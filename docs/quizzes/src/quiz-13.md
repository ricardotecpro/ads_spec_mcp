# Quiz 13 - Testes e Validação 🧪

1. Qual a importância dos Testes Unitários em um servidor MCP?
    - [ ] Garantir que o ícone do servidor seja o correto.
    - [x] Validar a lógica interna das ferramentas (Tools) de forma isolada do modelo de IA.
    - [ ] Substituir a necessidade de uma inteligência artificial.
    - [ ] Aumentar o preço do software.
    *Explicação: Testes unitários garantem que o "motor" das ferramentas funciona corretamente.*

2. O que o "MCP Inspector" permite validar?
    - [ ] A velocidade da conexão de internet.
    - [x] O Handshake, a listagem de recursos e a execução manual de ferramentas.
    - [ ] O design das janelas do Windows.
    - [ ] A qualidade do código em Python apenas.
    *Explicação: O Inspector é o parceiro ideal do desenvolvedor para testar a comunicação Cliente-Servidor.*

3. O que é um "Trigger Test" no contexto de IA e MCP?
    - [ ] Um teste de resistência física do computador.
    - [x] Verificar se a IA decide chamar a ferramenta correta para uma determinada pergunta do usuário.
    - [ ] Um comando para apagar todos os arquivos.
    - [ ] Uma forma de treinar a bateria do celular.
    *Explicação: Trigger tests validam se a descrição da ferramenta é clara para a IA.*

4. Por que o monitoramento de "Error Rate" é vital em produção?
    - [ ] Para saber quantos erros de português a IA comete.
    - [x] Para identificar se uma ferramenta está falhando constantemente por bugs ou parâmetros errados.
    - [ ] Para aumentar a memória RAM do servidor.
    - [ ] Para desligar o servidor automaticamente.
    *Explicação: Altas taxas de erro indicam que algo precisa ser consertado no código ou no prompt.*

5. O que significa "Mocking" em testes de servidores MCP?
    - [ ] Debochar do código de outros desenvolvedores.
    - [x] Simular a resposta de um serviço externo (como um banco de dados) para testar o servidor sem depender dele.
    - [ ] Usar uma IA de brinquedo no teste.
    - [ ] Trocar as fotos do projeto.
    *Explicação: Mocks permitem testar o servidor de forma isolada e previsível.*

6. Qual o código de erro para "Parse Error" no JSON-RPC?
    - [ ] `-32601`
    - [ ] `-32602`
    - [x] `-32700`
    - [ ] `-32000`
    *Explicação: `-32700` indica que o servidor recebeu um JSON com sintaxe inválida.*

7. Como os "Evals" (Avaliações) diferem dos testes de software tradicionais?
    - [ ] Evals são gratuitos, testes de software não.
    - [x] Evals medem a qualidade e a precisão da resposta da IA, que é subjetiva e probabilística.
    - [ ] Evals só funcionam com Claude 3.5.
    - [ ] Não há diferença, são apenas nomes novos.
    *Explicação: Testar IAs exige validar se a resposta "faz sentido", não apenas se o código rodou.*

8. O que é um teste de "Idempotência"?
    - [ ] Testar se o servidor fala várias línguas.
    - [x] Garantir que chamar a mesma ferramenta duas vezes com o mesmo dado não gere duplicidade indesejada (ex: dois pagamentos).
    - [ ] Verificar se o servidor é invisível.
    - [ ] Testar a cor da interface.
    *Explicação: Ferramentas seguras devem lidar com repetições sem causar danos.*

9. Qual a importância de logs de `stderr` bem detalhados?
    - [ ] Deixar o terminal mais colorido.
    - [x] Facilitar o rastreamento do erro exato quando uma ferramenta falha durante o uso da IA.
    - [ ] Esconder os bugs dos usuários.
    - [ ] Aumentar o tamanho do arquivo logs.txt.
    *Explicação: Logs claros reduzem drasticamente o tempo de manutenção.*

10. No desenvolvimento de um servidor MCP, o que "Validação de Schema" garante?
    - [ ] Que o servidor tenha um logotipo bonito.
    - [x] Que os dados trocados entre Cliente e Servidor sigam rigorosamente os tipos definidos (string, number, etc.).
    - [ ] Que a internet não caia durante o teste.
    - [ ] Que a IA não use palavras proibidas.
    *Explicação: A validação de schema é o "filtro" técnico que impede dados lixo no sistema.*
