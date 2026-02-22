# Projeto 09 - Otimizador de Prompts para Tools 🧠

## Objetivo
Refinar as capacidades de um servidor MCP através da Engenharia de Prompt, garantindo que a IA use as ferramentas com precisão cirúrgica.

## Requisitos
- Servidor MCP com pelo menos 3 Tools complexas.

## Atividades
1. **Auditoria de Falhas**: Peça à IA para realizar uma tarefa vaga. Note se ela chama a ferramenta errada ou com argumentos errados.
2. **Refinamento de Descrição**: Reescreva as descrições das Tools usando técnicas de "Chain of Thought" e "Role Prompting" dentro das strings de descrição.
3. **Prompt Template**: Crie um template de prompt no servidor que instrua a IA a sempre validar os dados com o usuário antes de executar a ferramenta.

## Entrega
- Documento comparativo (Antes vs Depois) das descrições das ferramentas.
- Feedback sobre a melhora na taxa de acerto da IA após o refinamento.

---

> [!TIP]
> Uma boa descrição explica: 1. O que a tool faz; 2. Quando usá-la; 3. O que os parâmetros significam em linguagem natural.