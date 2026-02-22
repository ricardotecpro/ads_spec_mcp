# Aula 10 - MCP com Aplicações Web 🌐

!!! tip "Objetivo"
    **Objetivo**: Compreender como integrar o protocolo MCP em aplicações frontend, criando interfaces ricas que permitem a interação entre o usuário final, modelos de IA e ferramentas de sistema.

---

## 1. O Fluxo de Comunicação na Web 🔄

Em uma aplicação web conectada ao MCP, o fluxo envolve um passo extra: o **Usuário**.

```mermaid
graph LR
    User[Usuário / Navegador] -- "Pergunta" --> App[App Web / Frontend]
    App -- "API / WebSocket" --> Client[MCP Client (Backend)]
    Client -- "Executa Tool" --> Server[MCP Server]
    Server -- "Resultado" --> Client
    Client -- "Gera Resposta" --> App
    App -- "Exibe UX" --> User
```

---

## 2. Bibliotecas e SDKs para Frontend 📦

Embora a maioria dos servidores MCP rode no backend (Node/Python), existem bibliotecas para facilitar a conversa com o front:

*   **MCP Web SDK**: Permite conexões via SSE diretamente do navegador (quando o servidor é remoto).
*   **Proxy-based**: O frontend conversa com um backend próprio, que atua como o Cliente MCP.

---

## 3. Experiência do Usuário (UX) Conectada 🎨

Diferente de um chat comum, uma aplicação MCP precisa mostrar o que está acontecendo "nos bastidores".

!!! concept "Transparência de Ação"
    1.  **Indicador de Chamada**: "IA está consultando o banco de dados..."
    2.  **Confirmação Humana**: "A IA deseja deletar este arquivo. Você autoriza?"
    3.  **Visualização de Dados**: Em vez de apenas texto, o frontend pode renderizar o JSON da Tool em um gráfico ou tabela bonita.

---

## 4. Segurança no Lado do Cliente (Frontend) 🛡️

*   **Não exponha Credenciais**: Nunca coloque chaves de API do seu Servidor MCP no código Javascript do frontend.
*   **Sanitização**: Filtre as respostas da IA antes de renderizá-las para evitar ataques de XSS (Cross-Site Scripting).

---

## 5. Prática: Dashboard de Ferramentas 💻

Imagine um frontend que lista as ferramentas disponíveis no seu Servidor MCP.

```termynal
$ npm run start-demo-app
[INFO] Servidor rodando em http://localhost:8080
[CONNECTED] Cliente MCP detectado.
[UI] Renderizando botões para as Tools:
  - [Check Weather]
  - [Send Email]
  - [Update CRM]
[SUCCESS] Clique e veja a IA agir no sistema!
```

---

## 6. Mini-Projeto: Assistente Web 🧪

1.  Desenhe um esboço de interface para um chat de suporte.
2.  Adicione um componente lateral que mostra quais "fontes de dados" (Resources) a IA está consultando no momento.
3.  Crie um botão de "Histórico de Ações" para que o usuário veja tudo o que o MCP executou durante a conversa.

---

## 7. Exercícios de Fixação 📝

1.  Por que é recomendável usar um backend como intermediário entre o Frontend e o Servidor MCP?
2.  Explique a importância da "Confirmação Humana" em aplicações web que usam MCP para ações destrutivas.
3.  Como a renderização de dados (gráficos/tabelas) melhora a percepção do usuário sobre o trabalho da IA?

---

!!! info "Dica"
    Use WebSockets para conexões de longa duração se o seu servidor MCP precisar enviar notificações de progresso em tempo real para o usuário.

**Próxima Aula**: [MCP e Arquitetura de Microsserviços](./aula-11.md) 🔌
