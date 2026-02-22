# Aula 15 - Projeto Prático Orientado 🎓
## Construindo um Sistema Inteligente Real

---

## Agenda de Hoje 📅

1. O Case: Assistente de RH Inteligente <!-- .element: class="fragment" -->
2. Modelagem das Tools e Resources <!-- .element: class="fragment" -->
3. Implementação Passo a Passo <!-- .element: class="fragment" -->
4. Testes e Ajustes Finos <!-- .element: class="fragment" -->
5. Apresentação do Resultado <!-- .element: class="fragment" -->

---

## 1. O Problema a Resolver 🚩

- Grande volume de candidatos. <!-- .element: class="fragment" -->
- Dificuldade em cruzar dados de currículos e vagas. <!-- .element: class="fragment" -->
- Necessidade de automação de feedbacks. <!-- .element: class="fragment" -->

---

## 2. Modelagem do Servidor

- **Resources**: Currículos (PDF/Text). <!-- .element: class="fragment" -->
- **Tools**: Comparar currículo com vaga, Enviar e-mail. <!-- .element: class="fragment" -->
- **Prompts**: Template de entrevista inicial. <!-- .element: class="fragment" -->

---

## 3. Arquitetura do Projeto

```mermaid
graph TD
    A[Claude Desktop] --> B[RH-MCP Server]
    B --> C[PDF Reader Service]
    B --> D[Email API]
    B --> E[(Banco de Talentos)]
```

---

## 4. Implementação: As Escolhas 🛠️

- Node.js + TypeScript. <!-- .element: class="fragment" -->
- SQLite para o banco local. <!-- .element: class="fragment" -->
- SDK MCP para as conexões. <!-- .element: class="fragment" -->

---

## 5. Prática: Construindo o Código 💻

```typescript
server.tool("avaliar_perfil", { cv: z.string(), vaga: z.string() }, 
  async ({ cv, vaga }) => {
    // Lógica de comparação...
  }
);
```

---

## 6. O Teste de Turing Prático 🤖

- A IA consegue dar um feedback justo? <!-- .element: class="fragment" -->
- O MCP forneceu todos os dados necessários? <!-- .element: class="fragment" -->

---

## 7. Documentando seu Projeto

- `README.md` completo. <!-- .element: class="fragment" -->
- Diagramas de fluxo. <!-- .element: class="fragment" -->
- Instruções de uso. <!-- .element: class="fragment" -->

---

## 8. Resumo ✅

- Projeto final consolida o aprendizado. <!-- .element: class="fragment" -->
- Integração real é o objetivo. <!-- .element: class="fragment" -->
- Documentação faz parte da engenharia. <!-- .element: class="fragment" -->

---

## 9. Próxima Aula: Futuro e Tendências ✨

- O que vem depois do MCP? <!-- .element: class="fragment" -->
- Ocupando o mercado de trabalho. <!-- .element: class="fragment" -->

---

## 10. Dúvidas? 🤔

> "Mãos à obra! A teoria sem prática é apenas um desejo."
