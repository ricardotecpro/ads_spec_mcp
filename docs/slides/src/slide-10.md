# Aula 10 - MCP com Aplicações Web 🌐
## Interfaces Modernas para Agentes de IA

---

## Agenda de Hoje 📅

1. Fluxo: Usuário -> IA -> MCP -> Web { .fragment }
2. Web SDKs e Conectividade { .fragment }
3. UX Transparente (Feedbacks Visuais) { .fragment }
4. Segurança no Frontend { .fragment }
5. Dashboards de Agents { .fragment }

---

## 1. O MCP no Navegador 🌍

- Aplicações web "AI-First". { .fragment }
- Conversas que resultam em ações na tela. { .fragment }

---

## 2. A Camada de Transporte SSE

- Server-Sent Events é nativo na web. { .fragment }
- Streaming de respostas da IA. { .fragment }

---

## 3. UX: O Padrão "Thinking" 💭

- Mostrar que a IA está trabalhando. { .fragment }
- "IA consultando logs..." { .fragment }
- Melhora a percepção de utilidade. { .fragment }

---

## 4. Segurança: Proxy e Backend 🛡️

```mermaid
graph LR
    A[Frontend] -- "WebSocket/SSE" --> B[Backend Node/Python]
    B -- "MCP Protocol" --> C[Servidores MCP]
    C -- "Ações" --> D[(Sistemas)]
```

---

## 5. Renderizando JSON de Ferramentas 🎨

- Em vez de texto bruto: Tabelas, Gráficos, Carrosséis. { .fragment }
- Cria interfaces muito mais ricas. { .fragment }

---

## 6. Confirmação do Usuário 👤

- Botão de "Executar Agora". { .fragment }
- Interceptação de ferramentas destrutivas. { .fragment }

---

## 7. Prática: Dashboard Simples 💻

- Listando ferramentas ativas em uma página web. { .fragment }

---

## 8. Arquitetura Web Distribuída

```mermaid
graph TD
    User --> WebApp
    WebApp --> Gateway[API Gateway / MCP Client]
    Gateway --> S1[Stock MCP]
    Gateway --> S2[User MCP]
    Gateway --> S3[Billing MCP]
```

---

## 9. Desafios de Latência

- Minimizar turnos de conversa. { .fragment }
- Cache agressivo no lado do cliente. { .fragment }

---

## 10. Resumo ✅

- SSE é o padrão para Web MCP. { .fragment }
- Transparência na UX é vital. { .fragment }
- Segurança exige backend intermediário. { .fragment }

---

## 11. Mini-Projeto: Esboço de UI

- Desenhar uma interface de chat que usa ferramentas MCP. { .fragment }

---

## 12. Dúvidas? 🤔

> "Interface é o que o usuário toca; Protocolo é o que faz funcionar."