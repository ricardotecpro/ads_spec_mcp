# Quiz 08 - Segurança no MCP 🔐

1. Qual o principal risco de um servidor MCP mal configurado?
    - [ ] O computador ficar muito bonito.
    - [x] Execução remota de comandos maliciosos e vazamento de dados privados.
    - [ ] A IA começar a falar em outra língua.
    - [ ] O aumento da velocidade do processador.
    *Explicação: A exposição de ferramentas dá poder real à IA, que pode ser abusada por inputs mal-intencionados.*

2. O que é "Prompt Injection"?
    - [ ] Injetar código Python no prompt.
    - [x] Uma técnica para enganar a IA e fazê-la ignorar suas regras de segurança.
    - [ ] Um método para melhorar a gramática da IA.
    - [ ] Enviar o prompt via e-mail.
    *Explicação: No MCP, um ataque de injection pode levar a IA a executar ferramentas que não deveria.*

3. Como o isolamento por "Sandboxing" (ex: Docker) ajuda na segurança?
    - [ ] Ele acelera a internet.
    - [x] Ele garante que, se o servidor for invadido, o invasor continue preso dentro de um ambiente limitado.
    - [ ] Ele apaga o vírus do sistema automaticamente.
    - [ ] Ele permite usar várias IAs ao mesmo tempo.
    *Explicação: O sandbox impede que uma falha no servidor comprometa toda a máquina hospedeira.*

4. Sobre "PII" (Personally Identifiable Information), o que o desenvolvedor MCP deve fazer?
    - [ ] Coletar o máximo possível para a IA ser inteligente.
    - [x] Identificar e omitir dados sensíveis como CPF, RG e senhas antes de enviá-los ao modelo.
    - [ ] Vender os dados para empresas de marketing.
    - [ ] Criptografar as informações com papel e caneta.
    *Explicação: Proteção de dados privados é uma obrigação ética e legal (GDPR/LGPD).*

5. O que significa "Zero Trust" em arquiteturas de IA e MCP?
    - [ ] Não confiar nem mesmo no próprio servidor.
    - [x] Verificar e autenticar rigorosamente cada requisição, independentemente de onde ela venha.
    - [ ] Acreditar que a IA nunca vai errar.
    - [ ] Desligar todos os sistemas de segurança.
    *Explicação: Em segurança moderna, a confiança nunca é presumida; ela é sempre validada.*

6. Por que usar caminhos absolutos e validados em ferramentas que leem arquivos?
    - [ ] Para o código ficar menor.
    - [x] Para evitar o ataque de "Path Traversal", onde a IA pode tentar ler arquivos sensíveis fora da pasta permitida.
    - [ ] Porque o Windows não entende caminhos relativos.
    - [ ] Para a IA ler os arquivos mais rápido.
    *Explicação: Validar caminhos impede que a IA acesse pastas como `/etc/passwd` ou `C:\Windows`.*

7. Qual a função do "Rate Limiting" em um servidor MCP público?
    - [ ] Limitar o número de usuários ativos.
    - [x] Limitar a quantidade de requisições por segundo para evitar ataques de negação de serviço (DoS).
    - [ ] Cobrar por cada pergunta feita à IA.
    - [ ] Diminuir a resolução das imagens enviadas.
    *Explicação: Limitar a taxa de chamadas protege a estabilidade e o custo da infraestrutura.*

8. O que é a "Aprovação Humana" (Human-in-the-loop)?
    - [ ] Um robô que vigia os humanos.
    - [x] Um mecanismo onde ações críticas só são executadas após o clique de confirmação de um ser humano.
    - [ ] A contratação de mais programadores.
    - [ ] Um curso de treinamento para IAs.
    *Explicação: É a última barreira de segurança para impedir que a IA delete dados ou envie e-mails errados.*

9. Ao rodar um servidor MCP remoto via HTTP/SSE, o que é indispensável?
    - [ ] Um monitor de 4K.
    - [x] Uso de protocolo seguro (HTTPS/TLS) para criptografar os dados em trânsito.
    - [ ] Que o servidor seja da cor azul.
    - [ ] Que o desenvolvedor fale inglês.
    *Explicação: Sem HTTPS, qualquer hacker na rede pode ler os dados JSON-RPC que viajam pela rede.*

10. No MCP, o que um servidor deve fazer se receber argumentos que não seguem o seu "Schema"?
    - [ ] Tentar processar de qualquer jeito.
    - [x] Rejeitar a requisição imediatamente e retornar um erro de "Invalid Params" (-32602).
    - [ ] Perguntar para a IA se ela tem certeza do que está fazendo.
    - [ ] Gravar um log e desligar o computador.
    *Explicação: Validação rigorosa de inputs é a primeira linha de defesa contra bugs e ataques.*
