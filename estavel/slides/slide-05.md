# Aula 05 - Comunicação Cliente ↔ Servidor 🔄
## Turnos, Mensagens e Fluxo de Dados

---

## Agenda de Hoje 📅

1. Requisições vs Notificações <!-- .element: class="fragment" -->
2. O Papel do ID na Comunicação <!-- .element: class="fragment" -->
3. Tratamento de Erros e Timeouts <!-- .element: class="fragment" -->
4. SSE (Server-Sent Events) na Prática <!-- .element: class="fragment" -->
5. Sampling: O Caminho Inverso <!-- .element: class="fragment" -->

---

## 1. Requisições (Requests) 📩

- Exigem uma resposta (Response). <!-- .element: class="fragment" -->
- Possuem um identificador único (`id`). <!-- .element: class="fragment" -->
- Blocos de construção das Tools. <!-- .element: class="fragment" -->

---

## 2. Notificações (Notifications) 📣

- "Fire and forget" (Dispare e esqueça). <!-- .element: class="fragment" -->
- Não possuem `id`. <!-- .element: class="fragment" -->
- Usadas para logs, progresso ou avisos. <!-- .element: class="fragment" -->

---

## 3. O Identificador de Requisição (ID)

```json
{
  "jsonrpc": "2.0",
  "method": "foo",
  "id": "abc-123"
}
```

- Essencial para conversas assíncronas. <!-- .element: class="fragment" -->
- Vincula a resposta à pergunta original. <!-- .element: class="fragment" -->

---

## 4. O Fluxo de Samplig 🔄

- O Servidor pede algo para o Cliente (IA). <!-- .element: class="fragment" -->
- "Gere um resumo deste artigo". <!-- .element: class="fragment" -->
- Inversão de papéis no MCP. <!-- .element: class="fragment" -->

---

## 5. Diagrama de Sampling

```mermaid
sequenceDiagram
    participant S as Servidor
    participant C as Cliente
    participant M as Modelo
    
    S->>C: mcp/sampling (prompt)
    C->>M: Gere texto solicitado
    M-->>C: Texto gerado
    C-->>S: Resposta do Sampling
```

---

## 6. Tratamento de Erros Técnicos ⚠️

- `-32700`: Parse Error. <!-- .element: class="fragment" -->
- `-32601`: Method not found. <!-- .element: class="fragment" -->
- `-32602`: Invalid params. <!-- .element: class="fragment" -->

---

## 7. Timeouts e Resiliência 🛡️

- O Cliente não espera para sempre. <!-- .element: class="fragment" -->
- Definição de limites de tempo saudáveis. <!-- .element: class="fragment" -->
- Tratamento de conexões interrompidas. <!-- .element: class="fragment" -->

---

## 8. SSE: Server-Sent Events 🌊

- Unidirecional (Servidor -> Cliente). <!-- .element: class="fragment" -->
- Perfeito para streaming de respostas e logs. <!-- .element: class="fragment" -->
- Menos complexo que WebSockets para IA. <!-- .element: class="fragment" -->

---

## 9. Prática: Inspecionando Requisições

```termynal
$ mcp-inspect call my_tool --debug
[SEND] --> {"id": 1, "method": "tools/call", ...}
[RECV] <-- {"id": 1, "result": {...}}
[SUCCESS] Ciclo completo!
```

---

## 10. Organização de Mensagens

```mermaid
graph TD
    A[Mensagem MCP] --> B(Request)
    A --> C(Notification)
    A --> D(Response)
    
    B --> B1[id, method, params]
    C --> C1[method, params]
    D --> D1[id, result/error]
```

---

## 11. O Papel do Stdio 📂

- Pipes de comunicação. <!-- .element: class="fragment" -->
- `stdin` para o servidor receber. <!-- .element: class="fragment" -->
- `stdout` para o servidor responder. <!-- .element: class="fragment" -->

---

## 12. Resumo ✅

- Requests exigem IDs e Respostas. <!-- .element: class="fragment" -->
- Notifications são apenas informativas. <!-- .element: class="fragment" -->
- Sampling permite que o servidor use a IA. <!-- .element: class="fragment" -->

---

## 13. Mini-Projeto: Log de Handshake

- Simular a sequência de initialize no papel. <!-- .element: class="fragment" -->

---

## 14. Dúvidas? 🤔

> "A clareza na comunicação evita o caos na implementação."
