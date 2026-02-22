# Quiz 10 - MCP com Aplicações Web 🌐

1. Qual o papel do navegador (browser) em uma aplicação web conectada ao MCP?
    - [ ] Ele é o servidor MCP.
    - [x] Ele serve como interface para o usuário interagir com o Cliente MCP.
    - [ ] Ele treina a IA em tempo real.
    - [ ] Ele armazena todos os modelos de linguagem.
    *Explicação: O navegador renderiza a UI onde o chat e as ferramentas são exibidas.*

2. Por que o transporte "HTTP with SSE" é crucial para apps web MCP?
    - [ ] Porque ele é mais antigo que o Stdio.
    - [x] Porque permite que o servidor envie atualizações de progresso em tempo real para o frontend.
    - [ ] Porque ele não exige o uso de JSON.
    - [ ] Porque ele só funciona em Macs.
    *Explicação: SSE (Server-Sent Events) é o padrão web para fluxos de dados do servidor para o cliente.*

3. O que é um "MCP Proxy" no desenvolvimento web?
    - [ ] Um vírus que rouba dados.
    - [x] Um backend intermediário que recebe chamadas do frontend e as encaminha para o servidor MCP real com segurança.
    - [ ] Uma forma de acelerar o Wi-Fi.
    - [ ] O nome do criador do protocolo.
    *Explicação: Proxies garantem que segredos (API Keys) nunca fiquem expostos no navegador.*

4. Qual a vantagem de renderizar os resultados de uma Tool em formato visual (graficos/cards) em vez de apenas texto?
    - [ ] Nenhuma, é apenas estética.
    - [x] Melhora a compreensão do usuário e torna a experiência da IA mais "tangível" e profissional.
    - [ ] Faz com que o servidor rode mais rápido.
    - [ ] Economiza bateria do servidor.
    *Explicação: UX rica é um diferencial de aplicações baseadas em Agents de IA.*

5. Sobre segurança web, por que nunca devemos colocar a chave do servidor MCP no arquivo `.js` do frontend?
    - [ ] Porque o arquivo ficaria muito grande.
    - [x] Porque qualquer usuário pode inspecionar o código e roubar a chave, ganhando acesso ao servidor.
    - [ ] Porque a chave só funciona em arquivos de texto.
    - [ ] Porque a IA não conseguiria ler a chave.
    *Explicação: Segredos de backend devem permanecer no backend.*

6. O que é "Transparência de Ação" na UX de uma aplicação MCP?
    - [ ] Deixar o fundo do aplicativo transparente.
    - [x] Mostrar visualmente quando a IA está consultando um servidor ou executando uma ferramenta.
    - [ ] Permitir que o usuário veja o código-fonte da IA.
    - [ ] Aumentar o brilho da tela.
    *Explicação: O usuário deve saber que a IA está agindo no sistema para evitar desconfiança.*

7. Como o protocolo MCP ajuda no desenvolvimento de "Micro-frontends" de IA?
    - [ ] Criando ícones bem pequenos.
    - [x] Permitindo que diferentes partes da tela sejam alimentadas por diferentes servidores MCP de forma modular.
    - [ ] Diminuindo o tamanho do arquivo HTML.
    - [ ] Substituindo o uso de CSS.
    - *Explicação: A modularidade do MCP combina perfeitamente com arquiteturas modulares de frontend.*

8. Qual o desafio de usar WebSockets em vez de SSE para MCP na web?
    - [ ] WebSockets são pretos e brancos.
    - [x] A complexidade de gerenciar o estado da conexão e bi-direcionalidade manual, enquanto o SSE é mais simples e nativo para streaming.
    - [ ] WebSockets não aceitam arquivos JSON.
    - [ ] WebSockets foram proibidos pelo Google.
    *Explicação: SSE é frequentemente preferido por ser mais leve e resiliente para fluxos de IA.*

9. O que acontece se o servidor MCP remoto cair em uma aplicação web?
    - [ ] O navegador do usuário explode.
    - [x] O frontend deve capturar o erro via cliente e avisar amigavelmente que a função está indisponível.
    - [ ] O usuário é desconectado da internet.
    - [ ] A IA começa a inventar dados aleatórios.
    *Explicação: Tratamento de erros de rede é vital para uma boa experiência do usuário.*

10. Como o MCP facilita o teste de interfaces de IA?
    - [ ] Testando a cor dos botões.
    - [x] Permitindo simular respostas do servidor MCP sem precisar de uma IA real conectada o tempo todo.
    - [ ] Aumentando o número de frames por segundo (FPS).
    - [ ] Traduzindo o site para braille.
    *Explicação: Mockar o servidor MCP permite validar a UI de forma rápida e barata.*
