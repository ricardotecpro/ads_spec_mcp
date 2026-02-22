# Quiz 02 - Fundamentos de Protocolos 📡

1. Qual protocolo de transporte o MCP utiliza como base para suas mensagens?
    - [ ] FTP
    - [ ] SMTP
    - [x] JSON-RPC 2.0
    - [ ] POP3
    *Explicação: O JSON-RPC é leve e focado em chamadas de métodos, ideal para o MCP.*

2. No formato JSON, como os dados são organizados?
    - [ ] Em tabelas de Excel.
    - [x] Em pares de chave e valor dentro de chaves `{}`.
    - [ ] Em parágrafos de texto corrido.
    - [ ] Em código Morse.
    *Explicação: O JSON usa estruturas de chave-valor (ex: "nome": "valor") para organizar dados.*

3. Qual a principal diferença entre REST e RPC?
    - [ ] REST é mais rápido que RPC.
    - [ ] RPC só funciona localmente.
    - [x] REST foca em Recursos (URLs), RPC foca em Ações (Métodos).
    - [ ] RPC não usa internet.
    *Explicação: REST lida com "substantivos" (recursos), RPC lida com "verbos" (chamar funções).*

4. O que é "Autenticação" no contexto de APIs?
    - [ ] Definir o que o usuário pode deletar.
    - [x] Validar a identidade de quem está acessando o sistema.
    - [ ] Medir a velocidade da conexão.
    - [ ] Trocar o nome do servidor.
    *Explicação: Autenticar é responder à pergunta: "Quem é você?".*

5. Qual formato de dados o MCP utiliza para garantir que humanos e máquinas entendam as mensagens?
    - [ ] XML
    - [ ] Binary
    - [x] JSON
    - [ ] YAML
    *Explicação: JSON foi escolhido por ser o padrão universal de troca de dados na web.*

6. No contexto de protocolos, o que é um "Contrato de Interface"?
    - [ ] Um documento assinado em cartório.
    - [x] Um acordo técnico sobre o formato e tipos de dados que serão trocados.
    - [ ] O contrato de trabalho do programador.
    - [ ] Uma regra que proíbe o uso de Java.
    *Explicação: O contrato define os campos obrigatórios e tipos (string, int) das mensagens.*

7. Para que servem os WebSockets em aplicações de IA?
    - [ ] Para economizar bateria do celular.
    - [x] Para permitir comunicação em tempo real e bi-direcional.
    - [ ] Para substituir o Wi-Fi.
    - [ ] Para criptografar arquivos de imagem.
    *Explicação: WebSockets mantêm a conexão aberta para fluxos contínuos de dados.*

8. O que acontece se uma mensagem JSON enviada ao MCP estiver malformada?
    - [ ] O servidor tenta adivinhar o que foi enviado.
    - [ ] O computador reinicia.
    - [x] O servidor retorna um erro de "Parse Error" (-32700).
    - [ ] A IA responde com um poema.
    *Explicação: O protocolo JSON-RPC exige sintaxe perfeita para processar requisições.*

9. Qual o papel da "Autorização"?
    - [ ] Verificar se o usuário está online.
    - [x] Verificar se o usuário autenticado tem permissão para uma ação específica.
    - [ ] Mudar a senha do banco de dados.
    - [ ] Instalar novos plugins.
    *Explicação: Autorizar é responder à pergunta: "O que você tem permissão de fazer?".*

10. Por que o JSON é mais popular que o XML em protocolos modernos?
    - [ ] Porque é mais antigo.
    - [x] Porque é mais leve, menos verboso e mais fácil de ler.
    - [ ] Porque só o JSON funciona no Windows.
    - [ ] Porque XML foi proibido pela Anthropic.
    *Explicação: A simplicidade do JSON o tornou o favorito para integrações ágeis.*
