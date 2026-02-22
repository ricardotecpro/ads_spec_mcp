# Quiz 07 - Integração com Banco de Dados 💾

1. Qual a principal recomendação ao expor um banco de dados para uma IA via MCP?
    - [ ] Dar acesso total com usuário `root`.
    - [x] Usar ferramentas parametrizadas e controladas em vez de queries SQL livres.
    - [ ] Desligar o firewall do banco.
    - [ ] Usar apenas planilhas TXT.
    *Explicação: Controle e segurança são fundamentais para evitar danos acidentais ou maliciosos.*

2. O que é "SQL Injection" no contexto de um servidor MCP?
    - [ ] Um método para acelerar as consultas.
    - [x] Um ataque onde comandos maliciosos são inseridos nos campos de busca para manipular o banco.
    - [ ] Uma vacina para servidores infectados.
    - [ ] Uma forma de backup automático.
    *Explicação: Inputs não tratados podem ser usados para deletar tabelas ou vazar dados.*

3. Como os "Prepared Statements" (queries parametrizadas) protegem o servidor?
    - [ ] Eles criptografam o banco de dados.
    - [x] Eles separam o comando SQL dos dados enviados, impedindo a execução de códigos extras.
    - [ ] Eles aumentam a memória RAM disponível.
    - [ ] Eles traduzem os nomes das colunas.
    *Explicação: Ao separar comando de dado, o banco de dados nunca trata o dado como parte da lógica.*

4. Qual a vantagem de usar um **Resource** para listar as tabelas de um banco?
    - [ ] É mais rápido que usar uma Tool.
    - [x] Permite que a IA conheça o esquema (colunas) antes de tentar fazer uma busca.
    - [ ] Oculta os dados reais dos usuários.
    - [ ] Economiza espaço de armazenamento.
    *Explicação: A IA precisa de contexto sobre a estrutura dos dados para perguntar corretamente.*

5. Sobre permissões de banco de dados, qual o princípio do "Privilégio Mínimo"?
    - [ ] Dar o máximo de acesso possível para não dar erro.
    - [ ] Criar apenas um usuário para toda a empresa.
    - [x] Fornecer apenas as permissões estritamente necessárias para o funcionamento da Tool.
    - [ ] Permitir que qualquer um delete o banco.
    *Explicação: Se a Tool só lê dados, o usuário do banco só deve ter permissão de `SELECT`.*

6. Se uma IA pedir para "Deletar todos os clientes inativos", o que é uma boa prática de UX no MCP?
    - [ ] Executar imediatamente para ser eficiente.
    - [ ] Ignorar o pedido sem avisar.
    - [x] Exigir uma confirmação humana clara antes de proceder com a ação destrutiva.
    - [ ] Deletar apenas metade para testar.
    *Explicação: Ações que alteram ou removem dados sensíveis devem ter supervisão humana.*

7. No SQLite, por que é comum usar o servidor MCP na mesma máquina do banco?
    - [ ] Porque SQLite não funciona em rede.
    - [x] Para aproveitar a baixa latência e a simplicidade de acesso direto ao arquivo `.db`.
    - [ ] Porque é o único banco que a Anthropic aceita.
    - [ ] Para economizar custos de eletricidade.
    *Explicação: SQLite é um banco baseado em arquivo, ideal para ferramentas locais rápidas.*

8. O que é "Introspecção de Esquema" (Schema Introspection)?
    - [ ] Uma técnica de meditação para programadores.
    - [x] O ato de consultar o banco para descobrir quais tabelas e colunas existem.
    - [ ] Mudar o nome do banco de dados a cada hora.
    - [ ] Apagar os índices das tabelas.
    *Explicação: É como a IA "lê o mapa" dos dados antes de navegar por eles.*

9. Por que não devemos expor colunas como `password_hash` no servidor MCP?
    - [ ] Porque a IA não saberia o que fazer com elas.
    - [x] Por motivos óbvios de segurança e privacidade do usuário.
    - [ ] Porque o JSON não aceita senhas.
    - [ ] Porque ocuparia muitos tokens de contexto.
    *Explicação: Dados sensíveis nunca devem chegar ao modelo de IA para evitar vazamentos.*

10. Qual a função dos logs de auditoria em um servidor MCP com banco de dados?
    - [ ] Aumentar o tamanho do disco rígido.
    - [x] Registrar exatamente quais consultas e ações a IA realizou para fins de fiscalização.
    - [ ] Ajudar a IA a aprender SQL mais rápido.
    - [ ] Substituir as tabelas de backup.
    *Explicação: Auditoria permite saber quem (ou qual IA) alterou o quê no sistema.*