# Projeto 14 - Dockerização e CI/CD 🚢

## Objetivo
Preparar um servidor MCP para produção usando containers e automação de deploy.

## Requisitos
- Docker instalado.
- Conta no GitHub.

## Atividades
1. **Dockerfile**: Crie um arquivo Dockerfile otimizado para seu servidor (use imagens Alpine para menor tamanho).
2. **GitHub Actions**: Configure um Workflow que:
    - Rode os testes automatizados (do Projeto 13).
    - Faça o build da imagem Docker.
    - Avise em caso de falha.
3. **Deploy Simulado**: Rode o container localmente e conecte o Claude Desktop a ele (usando `docker exec` ou apontando para o binário do docker).

## Entrega
- Arquivos `Dockerfile` e `.github/workflows/deploy.yml`.
- Print do comando `docker ps` mostrando o servidor rodando.

---

> [!IMPORTANT]
> Lembre-se de usar `.dockerignore` para não incluir a pasta `node_modules` ou arquivos `.env` na imagem.