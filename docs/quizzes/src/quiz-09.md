# Quiz 09 - MCP e Engenharia de Prompt 🧠

1. Por que a descrição de uma Tool no servidor MCP é considerada parte da "Engenharia de Prompt"?
    - [ ] Porque ela precisa ser escrita em rimas.
    - [x] Porque é essa descrição que ensina ao modelo de IA quando e como usar a ferramenta.
    - [ ] Porque ela define a cor do ícone da ferramenta.
    - [ ] Porque ela aumenta a quantidade de parâmetros do modelo.
    *Explicação: A descrição funciona como as instruções do System Prompt para o modelo.*

2. No MCP, o que acontece durante a "Injeção Dinâmica de Contexto"?
    - [ ] A IA injeta código malicioso no servidor.
    - [x] Dados de recursos (Resources) são inseridos automaticamente no prompt da IA para fornecer contexto atualizado.
    - [ ] O servidor aumenta o uso da CPU da IA.
    - [ ] O usuário é obrigado a digitar comandos técnicos.
    *Explicação: Injection no MCP é o ato de fornecer dados em tempo real para enriquecer a inteligência da IA.*

3. Qual a característica de uma descrição de Tool "AI-Friendly"?
    - [ ] É muito curta e usa siglas técnicas.
    - [x] É clara, específica e explica o "porquê" e o "quando" usar a ferramenta.
    - [ ] Não possui descrição, apenas o nome da função.
    - [ ] É escrita em código binário.
    *Explicação: Clareza e detalhamento ajudam o modelo a não cometer erros de julgamento.*

4. Como os "Prompt Templates" do MCP ajudam a reduzir a carga cognitiva da IA?
    - [ ] Fazendo com que a IA durma mais.
    - [x] Fornecendo uma estrutura de instrução já testada e otimizada, exigindo menos esforço da IA para entender a tarefa.
    - [ ] Substituindo a IA por um script fixo.
    - [ ] Escondendo as ferramentas do usuário.
    *Explicação: Templates garantem que a IA receba as melhores instruções possíveis para aquela função.*

5. O que é o "Context Window" (Janela de Contexto) e como o MCP interage com ela?
    - [ ] É a tela do monitor do usuário.
    - [x] É o limite de memória de curto prazo da IA; o MCP ajuda a preencher esse espaço com informações externas relevantes.
    - [ ] É o tempo que a IA demora para carregar.
    - [ ] É a pasta onde ficam os arquivos de configuração.
    *Explicação: O MCP fornece os dados "frescos" que entram na janela de contexto do modelo.*

6. Por que devemos evitar nomes genéricos como `save_data` em servidores MCP com muitas ferramentas?
    - [ ] Porque o nome é feio.
    - [x] Para evitar que a IA se confunda entre ferramentas similares de diferentes servidores.
    - [ ] Porque nomes longos são mais rápidos para o computador ler.
    - [ ] É uma regra apenas para o Windows.
    *Explicação: Nomes específicos como `save_customer_contact` reduzem a chance de erro da IA.*

7. No MCP, o que significa fornecer "Few-shot examples" em um Prompt Template?
    - [ ] Dar poucos tiros em um jogo de tiro da IA.
    - [x] Fornecer alguns exemplos de entrada e saída esperada para que a IA aprenda o padrão de resposta.
    - [ ] Limitar a IA a responder apenas uma frase.
    - [ ] Usar apenas modelos pequenos (Small Language Models).
    *Explicação: Exemplos ajudam a IA a entender o formato e o tom de voz desejados.*

8. Qual o impacto de uma descrição de Tool mal escrita?
    - [ ] O servidor para de funcionar tecnicamente.
    - [x] A IA pode "alucinar" (chamar a ferramenta na hora errada ou com dados errados).
    - [ ] A internet fica lenta para o usuário.
    - [ ] O código-fonte do servidor é deletado.
    *Explicação: Se a IA não entender o propósito, ela usará a ferramenta de forma incorreta.*

9. Como o "RAG" se beneficia do MCP na Engenharia de Prompt?
    - [ ] O RAG deixa de existir.
    - [x] O MCP fornece um canal padronizado para a recuperação dos documentos que o RAG precisa.
    - [ ] O MCP treina o modelo para não precisar de RAG.
    - [ ] O RAG se torna mais caro com o MCP.
    *Explicação: O MCP é o "conector" ideal para arquiteturas de RAG (Retrieval-Augmented Generation).*

10. O que é "System Prompt Tuning" aplicado ao MCP?
    - [ ] Ajustar a cor da interface do sistema.
    - [x] Refinar as instruções globais da IA para que ela saiba priorizar e usar corretamente as capacidades do servidor MCP.
    - [ ] Aumentar a velocidade do sistema operacional.
    - [ ] Trocar o servidor MCP por uma planilha Excel.
    *Explicação: O tuning foca em calibrar a inteligência para o uso otimizado do protocolo.*