# Quiz 11 - MCP e Microsserviços 🔌

1. Qual a principal vantagem de usar MCP em uma arquitetura de Microsserviços?
    - [ ] Diminuir o número de servidores.
    - [x] Permitir que a IA orquestre e acesse múltiplos serviços independentes de forma padronizada.
    - [ ] Substituir o uso de bancos de dados.
    - [ ] Usar apenas uma linguagem de programação para tudo.
    *Explicação: O MCP serve como a "cola" inteligente entre diversos microsserviços.*

2. O que é um "Gateway MCP" em sistemas distribuídos?
    - [ ] Um porteiro humano para o data center.
    - [x] Um ponto central que recebe requisições de IA e as roteia para o microsserviço/servidor MCP correto.
    - [ ] Uma marca de roteador para servidores.
    - [ ] Um comando para deletar toda a rede.
    *Explicação: Gateways simplificam o acesso da IA a sistemas complexos com muitos servidores.*

3. Sobre a escalabilidade de servidores MCP, o que significa "Horizontal Scaling"?
    - [ ] Aumentar o tamanho do servidor fisicamente.
    - [x] Adicionar mais instâncias de um servidor MCP para dividir a carga de trabalho.
    - [ ] Deitar o servidor de lado para economizar espaço.
    - [ ] Trocar o servidor de lugar na sala.
    *Explicação: Escalar horizontalmente protege o sistema contra picos de uso.*

4. Por que o **Desacoplamento** é benéfico no ecossistema MCP?
    - [ ] Porque as peças do computador ficam mais soltas.
    - [x] Porque permite atualizar um servidor MCP específico sem derrubar os outros.
    - [ ] Porque diminui a segurança do sistema.
    - [ ] Porque impede que os serviços se comuniquem.
    *Explicação: Mudanças isoladas reduzem o risco de falhas em cascata.*

5. O que os "Health Checks" (Verificações de Saúde) fazem em um ambiente MCP?
    - [ ] Verificam se o programador está doente.
    - [x] Monitoram periodicamente se os servidores MCP estão vivos e respondendo corretamente.
    - [ ] Contam quantas calorias o computador consome.
    - [ ] Limpam os arquivos temporários.
    *Explicação: Health checks garantem que a IA não tente usar um servidor que está offline.*

6. Qual o papel do "Service Discovery" (Descoberta de Serviço) no MCP?
    - [ ] Procurar por novas IAs no Google.
    - [x] Automatizar a localização das URLs dos diversos servidores MCP na rede para o Cliente.
    - [ ] Descobrir quem escreveu o código malicioso.
    - [ ] Encontrar arquivos deletados.
    *Explicação: Em redes complexas, as URLs mudam; a descoberta automática evita configurações manuais.*

7. Como o **Correlation ID** ajuda no monitoramento do MCP?
    - [ ] Identifica a cor do ícone do servidor.
    - [x] Permite rastrear uma única pergunta do usuário através de todos os servidores MCP chamados pela IA.
    - [ ] Melhora a velocidade da tradução.
    - [ ] Serve como senha mestra.
    *Explicação: Tracing distribuído é essencial para debugar fluxos complexos de agentes de IA.*

8. O que acontece se um Microsserviço demorar muito a responder a uma ferramenta MCP?
    - [ ] O sistema todo trava para sempre.
    - [x] O Cliente MCP dispara um erro de "Timeout" e a IA deve lidar com a indisponibilidade.
    - [ ] A internet do usuário cai.
    - [ ] O servidor reinicia sozinho.
    *Explicação: Timeouts protegem a experiência do usuário contra serviços lentos.*

9. Por que o MCP é preferível a criar APIs Customizadas para cada Microsserviço?
    - [ ] Porque é mais caro.
    - [x] Pela padronização: a IA já sabe "como falar" MCP, eliminando o custo de ensinar cada nova API.
    - [ ] Porque APIs customizadas foram proibidas pela ONU.
    - [ ] Porque o MCP é feito de ouro digital.
    *Explicação: Padrões aceleram o desenvolvimento e reduzem a manutenção.*

10. No contexto de microsserviços, o que é um servidor MCP "Stateless" (Sem Estado)?
    - [ ] Um servidor que não tem país.
    - [x] Um servidor que não guarda dados na memória local entre requisições, facilitando a escalabilidade.
    - [ ] Um servidor que está sempre desligado.
    - [ ] Um servidor que não usa banco de dados.
    *Explicação: Stateless permite que qualquer instância do servidor atenda qualquer pedido.*
