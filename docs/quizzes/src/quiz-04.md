# Quiz 04 - Estrutura de Recursos no MCP 📂

1. O que são "Resources" no Model Context Protocol?
    - [ ] Botões que a IA pode apertar.
    - [x] Dados de leitura disponibilizados pelo servidor (ex: arquivos, logs).
    - [ ] A memória RAM do modelo de linguagem.
    - [ ] Gráficos gerados pela IA.
    *Explicação: Resources funcionam como "documentos" que a IA pode consultar.*

2. Qual a principal diferença entre uma "Tool" e um "Resource"?
    - [ ] Tools são pagas, Resources são grátis.
    - [ ] Resources são caminhos, Tools são nomes.
    - [x] Resources são para leitura de dados, Tools são para executar ações (escrever/mudar algo).
    - [ ] Não há diferença técnica.
    *Explicação: Tools realizam transformações ou ações no mundo real; Resources são informativos.*

3. O que é uma URI no contexto de Resources?
    - [ ] Um segredo de estado.
    - [x] Um identificador único (como uma URL) para localizar o recurso no servidor.
    - [ ] A versão do protocolo MCP.
    - [ ] O nome do modelo de IA.
    *Explicação: URIs (ex: mcp://server/log) identificam exatamente qual dado deve ser lido.*

4. Para que servem os "Prompts" registrados em um servidor MCP?
    - [ ] Para salvar a senha do usuário.
    - [x] Para fornecer templates de instruções pré-configurados para a IA.
    - [ ] Para aumentar a velocidade da internet.
    - [ ] Para traduzir o site para chinês.
    *Explicação: Prompts ajudam a padronizar como a IA executa tarefas específicas.*

5. O que é um "Dynamic Resource"?
    - [ ] Um dado que nunca muda.
    - [x] Um recurso cujo conteúdo é gerado ou atualizado em tempo real no momento da leitura.
    - [ ] Um vídeo que a IA consegue assistir.
    - [ ] Uma ferramenta de animação 3D.
    *Explicação: O conteúdo de um recurso dinâmico reflete o estado atual dos dados.*

6. Por que a "Descrição" de uma Tool é tão importante?
    - [ ] Porque fica bonita na documentação.
    - [x] Porque é através dela que o Modelo (LLM) decide se deve ou não chamar a ferramenta.
    - [ ] Para que o usuário saiba quanto vai custar a ferramenta.
    - [ ] Não é importante, apenas o nome importa.
    *Explicação: A descrição é o prompt que ensina a IA a utilidade da ferramenta.*

7. O que acontece na fase de "Descoberta" (Discovery)?
    - [ ] O usuário descobre novas IAs na internet.
    - [x] O Cliente lista todas as Tools, Resources e Prompts que o servidor oferece.
    - [ ] O servidor tenta descobrir a senha do Wi-Fi.
    - [ ] A IA descobre o sentido da vida.
    *Explicação: Discovery é o momento em que o "cardápio" do servidor é apresentado ao cliente.*

8. O que é o "JSON Schema" em uma definição de Tool?
    - [ ] Um desenho do logotipo do projeto.
    - [x] A definição técnica obrigatória dos tipos e formatos de argumentos que a ferramenta aceita.
    - [ ] Uma lista de nomes de desenvolvedores.
    - [ ] Um comando para deletar arquivos JSON.
    *Explicação: O Schema garante que a IA envie os dados no formato correto (número, texto, etc.).*

9. No MCP, o que significa o prefixo `mcp://`?
    - [ ] Que o site é seguro (HTTPS).
    - [x] É o esquema padrão de URI para identificar recursos e capacidades do protocolo.
    - [ ] Que a mensagem foi escrita por uma IA.
    - [ ] É um erro de digitação de `http://`.
    *Explicação: É a forma padronizada de endereçar itens dentro do ecossistema MCP.*

10. Pode um servidor MCP oferecer apenas Tools e nenhum Resource?
    - [ ] Não, é proibido pelo protocolo.
    - [x] Sim, um servidor pode expor qualquer combinação de capacidades (ou até nenhuma).
    - [ ] Sim, mas apenas se for pago.
    - [ ] Não, a IA ficaria confusa.
    *Explicação: A arquitetura do MCP é modular e flexível para diversas necessidades.*
