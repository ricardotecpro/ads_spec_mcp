# Quiz 12 - Tratamento de Estado e Contexto 🔑

1. O que é o "Estado" (State) em um servidor MCP?
    - [ ] O país onde o servidor está localizado.
    - [x] A capacidade do servidor de lembrar informações ou manter o contexto de uma conversa.
    - [ ] A cor da janela do terminal.
    - [ ] O nível de bateria do computador.
    *Explicação: Estado é a "memória" do sistema sobre o que aconteceu anteriormente.*

2. Qual a diferença entre Memória Transiente e Memória Persistente?
    - [ ] Transiente é mais lenta que Persistente.
    - [x] Transiente apaga ao reiniciar; Persistente é salva em disco/banco de dados para sempre.
    - [ ] Persistente só funciona em Python.
    - [ ] Não há diferença técnica.
    *Explicação: Persistência é necessária para recordar preferências do usuário em dias diferentes.*

3. Por que o gerenciamento de sessões (`session_id`) é fundamental para IAs multi-usuário?
    - [ ] Para cobrar os usuários corretamente.
    - [x] Para garantir que a IA não confunda os dados e o contexto de diferentes usuários no mesmo servidor.
    - [ ] Para mudar a língua da IA para cada usuário.
    - [ ] Para permitir que os usuários conversem entre si.
    *Explicação: Isolamento de sessão é uma regra básica de privacidade e segurança.*

4. O que é a técnica de "Context Window Pruning" (Poda da Janela de Contexto)?
    - [ ] Deletar os arquivos do servidor para abrir espaço.
    - [x] Remover informações irrelevantes ou antigas para manter apenas o essencial dentro do limite de memória da IA.
    - [ ] Cortar os fios do computador.
    - [ ] Diminuir as letras das mensagens.
    *Explicação: Manter o contexto "limpo" ajuda a IA a ser mais precisa e barata.*

5. Sobre a "Persistência Semântica", para que servem as Bases de Dados Vetoriais?
    - [ ] Para desenhar vetores matemáticos na tela.
    - [x] Para permitir que a IA busque memórias passadas por similaridade de significado, não apenas por palavras exatas.
    - [ ] Para aumentar o volume do som do computador.
    - [ ] Para criptografar os logs do servidor.
    *Explicação: Busca vetorial é o coração da "memória de longo prazo" moderna para IAs.*

6. O que é um "Token" e como ele afeta o estado da IA?
    - [ ] Uma moeda virtual para comprar IAs.
    - [x] A unidade básica de processamento de texto da IA; quanto mais tokens no estado, mais caro e lento o processamento.
    - [ ] Um comando de segurança para desligar o servidor.
    - [ ] O nome do mascote do MCP.
    *Explicação: Gerenciar o número de tokens no contexto é essencial para a eficiência.*

7. Como o MCP ajuda na "Recuperação de Contexto" (RAG)?
    - [ ] Fazendo com que a IA adivinhe os dados.
    - [x] Fornecendo ferramentas padronizadas para buscar documentos externos e injetá-los na conversa na hora certa.
    - [ ] Deletando o histórico de conversas.
    - [ ] Traduzindo os documentos para latim.
    *Explicação: O MCP é o veículo pelo qual o contexto externo chega até o modelo.*

8. O que é "Summarization" (Resumo) de Histórico?
    - [ ] Apagar o histórico e começar do zero.
    - [x] Condensar conversas longas em um pequeno resumo para economizar espaço de contexto e memória.
    - [ ] Mudar a fonte do texto para o tamanho 8.
    - [ ] Gravar a conversa em um CD-ROM.
    *Explicação: Resumir permite manter os fatos importantes sem usar milhares de tokens.*

9. Qual o risco de manter muito estado (muita memória) no servidor MCP?
    - [ ] O servidor ficar muito inteligente.
    - [x] Aumento do consumo de RAM, latência e risco de vazamento de informações obsoletas.
    - [ ] O computador ficar muito pesado fisicamente.
    - [ ] A IA parar de falar.
    *Explicação: Eficiência e "limpeza" de dados são boas práticas de engenharia.*

10. No MCP, o que significa um servidor "Idempotente"?
    - [ ] Um servidor que nunca responde.
    - [x] Um servidor onde executar a mesma ferramenta várias vezes com o mesmo dado não causa efeitos colaterais extras indesejados.
    - [ ] Um servidor que só funciona uma vez por dia.
    - [ ] Um servidor que é invisível na rede.
    *Explicação: Idempotência evita erros caso a IA repita uma ação por esquecer que já a fez.*
