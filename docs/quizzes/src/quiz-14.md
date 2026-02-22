# Quiz 14 - Deploy de Servidor MCP 🚢

1. Qual a principal vantagem de usar Docker para o deploy de um servidor MCP?
    - [ ] Deixa o servidor mais rápido que o normal.
    - [x] Garante que o servidor rode de forma idêntica em qualquer ambiente (local, nuvem, etc.).
    - [ ] Permite que o servidor nade na internet.
    - [ ] Diminui o custo da eletricidade do servidor.
    *Explicação: Docker isola as dependências e o sistema operacional, evitando o erro "funciona na minha máquina".*

2. Por que variáveis de ambiente (`.env`) são preferíveis a "Hardcoded values" no deploy?
    - [ ] Porque elas são mais fáceis de digitar.
    - [x] Para manter segredos (chaves de API, senhas) fora do código e facilitar mudanças em diferentes ambientes.
    - [ ] Porque a IA não consegue ler variáveis de ambiente.
    - [ ] Porque é uma lei internacional de programação.
    *Explicação: Segurança e flexibilidade são os pilares do uso de variáveis de ambiente.*

3. O que é um "CI/CD Pipeline" aplicado ao MCP?
    - [ ] Um cano que leva dados do servidor para a IA.
    - [x] Um processo automatizado de Build, Teste e Deploy do servidor a cada mudança no código.
    - [ ] Uma forma de carregar a bateria do servidor.
    - [ ] O nome do criador do Docker.
    *Explicação: CI/CD garante que apenas versões testadas e estáveis cheguem à produção.*

4. Qual a diferença entre deploy em Stdio e deploy em SSE (HTTP)?
    - [ ] Stdio é para fotos, SSE é para vídeos.
    - [x] Stdio é para uso local (mesma máquina); SSE permite acesso remoto via rede/internet.
    - [ ] SSE é gratuito e Stdio é pago.
    - [ ] Não há diferença, ambos são iguais.
    *Explicação: A escolha do transporte define se o servidor é privado ou distribuído.*

5. Sobre infraestrutura de nuvem, o que é o "Render" ou "Fly.io"?
    - [ ] Marcas de monitores de vídeo.
    - [x] Plataformas de hospedagem (PaaS) que facilitam o deploy de containers Docker e servidores SSE.
    - [ ] Sistemas operacionais novos para IAs.
    - [ ] Aplicativos para editar imagens.
    *Explicação: Estas plataformas simplificam o deploy remoto para desenvolvedores.*

6. Por que o isolamento de rede (Firewall) é importante para servidores MCP remotos?
    - [ ] Para aumentar a velocidade do Wi-Fi.
    - [x] Para garantir que apenas clientes autorizados consigam se conectar ao seu servidor e suas ferramentas.
    - [ ] Para mudar a IP do servidor.
    - [ ] Para impedir que a IA acesse o Google.
    *Explicação: Servidores MCP podem ter acesso a dados sensíveis; o acesso deve ser restrito.*

7. No Dockerfile, o que o comando `CMD` faz?
    - [ ] Deleta os arquivos da pasta atual.
    - [x] Define qual comando será executado quando o container for iniciado.
    - [ ] Muda o nome do container.
    - [ ] Instala o Windows dentro do Docker.
    *Explicação: Sem o `CMD`, o container sobe mas não inicia o seu servidor MCP.*

8. O que é um "Registry" de containers (como o Docker Hub)?
    - [ ] Um livro onde se registra o nome dos programadores.
    - [x] Um armazém online onde as imagens Docker do seu servidor ficam guardadas para o deploy.
    - [ ] Um site para comprar servidores usados.
    - [ ] Uma lista de ferramentas do MCP.
    *Explicação: O registry é o ponto de distribuição das suas imagens prontas para uso.*

9. No deploy, o que significa "Zero Downtime"?
    - [ ] O servidor nunca desliga, mesmo sem internet.
    - [x] Atualizar o servidor com uma versão nova sem que o usuário perceba queda no serviço.
    - [ ] O servidor não usa bateria.
    - [ ] A IA responde em 0 segundos.
    *Explicação: É essencial para manter a IA disponível 24/7 para seus usuários.*

10. Qual a função de um "Healthcheck" em um servidor Dockerizado?
    - [ ] Medir a temperatura do processador.
    - [x] Informar ao orquestrador (Docker/Kubernetes) se o processo do servidor MCP ainda está rodando e saudável.
    - [ ] Limpar a memória RAM do container.
    - [ ] Traduzir mensagens de erro para o inglês.
    *Explicação: Se o healthcheck falha, o sistema pode reiniciar o servidor automaticamente.*
