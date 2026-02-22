# Projeto 12 - Memória de Longo Prazo com Redis 💾

## Objetivo
Implementar persistência de estado em um servidor MCP, permitindo que a IA se lembre de preferências do usuário entre diferentes conversas.

## Requisitos
- Banco Redis (pode ser local ou via Cloud como Upstash).
- Node.js ou Python.

## Atividades
1. **Identificação de Sessão**: Crie um middleware que captura o ID do usuário/sessão.
2. **Ferramentas de Memória**:
    - `remember_preference(key, value)`: Salva no Redis.
    - `recall_preferences()`: Lê do Redis e injeta no contexto da IA.
3. **Teste de Persistência**: Reinicie seu servidor e verifique se a IA ainda sabe as preferências salvas anteriormente.

## Entrega
- Código-fonte da integração com o Redis.
- Demonstração do servidor mantendo o estado após um shutdown.

---

> [!TIP]
> Use o tempo de vida (TTL) do Redis para evitar que a memória do servidor fique sobrecarregada com dados antigos.