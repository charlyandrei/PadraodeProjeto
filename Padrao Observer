# Padrão Projeto Observer
1.Pattern Name and Classification

O padrão Observer funciona como assinaturas de jornais e revistas, ou seja, temos uma editora que publica as edições e pessoas que assinam os jornais ou revistas dessa editora e sempre recebem as novas edições assim que elas são publicadas. Enquanto a pessoa é assinante ela continua recebendo as edições na sua casa. Se a pessoa cancelar a assinatura do jornal ou da revista ela para de receber as edições.

  -Intent
  Define uma dependência um-para-muitos entre objetos para que, quando um objeto muda de estado, todos os seus dependentes sejam notificados e atualizados automaticamente.
  
  - Motivation
  
    Não podemos falar sobre Programação Orientada a Objetos sem considerar o estado dos objetos. Afinal, a programação orientada a objetos trata de objetos e sua interação. São frequentes os casos em que determinados objetos precisam ser informados sobre as alterações ocorridas em outros objetos. Ter um bom design significa desacoplar o máximo possível e reduzir as dependências. O Observer Design Pattern pode ser usado sempre que um assunto tiver que ser observado por um ou mais observadores.
    Vamos supor que temos um sistema de estoque que fornece dados para vários tipos de clientes. Queremos ter um cliente implementado como um aplicativo baseado na web, mas em um futuro próximo precisamos adicionar clientes para dispositivos móveis, Palm ou Pocket PC, ou ter um sistema para notificar os usuários com alertas de sms. Agora é simples ver o que precisamos do padrão de observador: precisamos separar o assunto (servidor de ações) de seus observadores (aplicativos cliente) de forma que a adição de um novo observador seja transparente para o servidor.

   - Applicability
     -O padrão do observador é usado quando:
     -A mudança de estado em um objeto deve ser refletida em outro objeto, sem manter os objetos fortemente acoplados.
     -A estrutura que estamos escrevendo precisa ser aprimorada no futuro com novos observadores com mudanças mínimas.
  
  - Structure 
 
 ![](https://refactoring.guru/images/patterns/diagrams/observer/structure.png)
  
  - Participants
  
   -A Publisher manda eventos de interesse para outros objetos. Esses eventos ocorrem quando a publicadora muda seu estado ou executa algum comportamento. As publicadoras contêm uma infraestrutura de inscrição que permite novos assinantes se juntar aos atuais assinantes ou deixar a lista.
   
   -O Client cria a publicadora e os objetos assinantes separadamente e então registra os assinantes para as atualizações da publicadora.
   
   -Concrete Subscribes realizam algumas ações em resposta às notificações enviadas pela publicadora. Todas essas classes devem implementar a mesma interface para que a publicadora não fique acoplada à classes concretas.
   
   -Client colabora com objetos em conformidade com a interface de destino.
  - Sample Code 
  
  (https://github.com/charlyandrei/PadraodeProjeto/blob/master/Code%20Observer)
