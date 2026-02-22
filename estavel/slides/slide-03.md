# Aula 03 - Arquitetura do MCP 🏗️
## Entendendo os Componentes e Fluxos

---

## Agenda de Hoje 📅

1. Cliente, Servidor e Modelo <!-- .element: class="fragment" -->
2. Métodos de Transporte (Stdio vs SSE) <!-- .element: class="fragment" -->
3. O Fluxo de Inicialização <!-- .element: class="fragment" -->
4. Cicatrizando a Comunicação <!-- .element: class="fragment" -->
5. Segurança por Design <!-- .element: class="fragment" -->

---

## 1. Os Três Atores Principais 🎭

```mermaid
graph TD
    A[Modelo - LLM] --- B[Cliente - Host]
    B --- C[Servidor - Source]
```

---

## 1.1 O Modelo (A Inteligência) 🧠

- Tome as decisões. <!-- .element: class="fragment" -->
- Analisa os dados recebidos. <!-- .element: class="fragment" -->
- Decide qual ferramenta chamar. <!-- .element: class="fragment" -->

---

## 1.2 O Cliente (O Orquestrador) 👷

- Conecta o modelo aos servidores. <!-- .element: class="fragment" -->
- Gerencia o estado e as permissões. <!-- .element: class="fragment" -->
- Ex: Claude Desktop, Cursor, IDEs. <!-- .element: class="fragment" -->

---

## 1.3 O Servidor (A Fonte) 💾

- Expor dados e funcionalidades. <!-- .element: class="fragment" -->
- Conecta ao mundo real (Arquivos, APIs, DB). <!-- .element: class="fragment" -->
- Rodam como processos isolados. <!-- .element: class="fragment" -->

---

## 2. Métodos de Transporte 🚀

---

## 2.1 Stdio (Standard I/O) 📂

- Comunicação local via terminais. <!-- .element: class="fragment" -->
- Muito seguro (isolado na máquina). <!-- .element: class="fragment" -->
- Baixa latência. <!-- .element: class="fragment" -->

---

## 2.2 SSE (HTTP + Server-Sent Events) ☁️

- Ideal para conexões remotas. <!-- .element: class="fragment" -->
- Escalonável na nuvem. <!-- .element: class="fragment" -->
- Exige tratamento de rede. <!-- .element: class="fragment" -->

---

## 3. Ciclo de Vida do Servidor 🔄

- Launch -> Initialize -> Run -> Shutdown. <!-- .element: class="fragment" -->

---

## 4. O Passo a Passo da Chamada

1. Modelo solicita `tool(args)`. <!-- .element: class="fragment" -->
2. Cliente valida e envia `Request`. <!-- .element: class="fragment" -->
3. Servidor executa e retorna `Result`. <!-- .element: class="fragment" -->
4. Cliente entrega `Result` para o Modelo. <!-- .element: class="fragment" -->

---

## 5. Diagrama de Sequência

```mermaid
sequenceDiagram
    participant M as Modelo
    participant C as Cliente
    participant S as Servidor
    
    M->>C: Desejo usar Tool X
    C->>S: tools/call (X)
    S-->>C: result (JSON)
    C->>M: Aqui está o dado
```

---

## 6. Isolamento e Segurança 🔐

- Servidores rodam como subprocessos. <!-- .element: class="fragment" -->
- Não afetam a estabilidade do Cliente. <!-- .element: class="fragment" -->
- Permissões granulares por ferramenta. <!-- .element: class="fragment" -->

---

## 7. Prática: Monitorando Processos

```termynal
$ ps -ef | grep mcp-server
root 1234 ... /usr/bin/node my-mcp-server.js
[INFO] Servidor rodando isolado.
```

---

## 8. Descoberta Dinâmica (Capabilities) 🔍

- O servidor diz ao cliente o que ele "sabe" fazer. <!-- .element: class="fragment" -->
- Permite extensibilidade sem mudar o código do cliente. <!-- .element: class="fragment" -->

---

## 9. Tratamento de Notificações 📩

- Mudança de estado sem interrupção. <!-- .element: class="fragment" -->
- Logs de depuração em tempo real. <!-- .element: class="fragment" -->

---

## 10. Resumo ✅

- Arquitetura desacoplada em 3 pilares. <!-- .element: class="fragment" -->
- Stdio para local, SSE para remoto. <!-- .element: class="fragment" -->
- Segurança centrada no Cliente. <!-- .element: class="fragment" -->

---

## 11. Mini-Projeto: Fluxograma

- Desenhar o fluxo de uma consulta ao banco via MCP. <!-- .element: class="fragment" -->

---

## 12. Dúvidas? 🤔

> "A arquitetura correta simplifica o impossível."