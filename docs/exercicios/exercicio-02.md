# Exercícios: Aula 02 - Fundamentos de Protocolos 📡

### 🟢 Nível Básico

1.  Diferencie brevemente **REST** de **RPC**.
2.  O que é um arquivo **JSON** e por que ele é usado no MCP?

### 🟡 Nível Intermediário

3.  Analise o JSON abaixo e identifique: o método chamado e os argumentos enviados.
    ```json
    {
      "method": "tools/call",
      "params": {
        "name": "get_stock_price",
        "arguments": { "ticker": "AAPL" }
      }
    }
    ```
4.  Qual a importância do "Contrato de Interface" para evitar que a IA receba dados em formatos inesperados?

### 🔴 Nível Desafio

5.  **Cenário de Segurança**: Um servidor MCP remoto exige autenticação. Como você estruturaria uma mensagem JSON para informar ao cliente que ele precisa fornecer uma credencial antes de listar os recursos? (Descreva a lógica ou o JSON).
