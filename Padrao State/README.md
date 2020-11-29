# Padrão Projeto State
#1.Pattern Name and Classification
- Padrão state
- Comportamental de Objetos

#Intent
  - Permitir que um objeto altere seu comportamento quando seu estado é alterado;
  - Alterar o comportamento de um objeto quando houver alguma mudança no seu estado interno, como se ele tivesse mudado de classe.
  - Separar os estados em classes encapsuladas e delega as tarefas para o objeto que representa o estado atual, e os comportamentos mudam juntamento com o estado interno.
  
#Motivation
  
  - É útil, pois o padrão encapsula os estados em classes separadas e delega as tarefas para o objeto que representa o estado atual.
  - Atente-se para somente utilizar as entidades de estado não static se seu projeto não trabalha com compartilhamento de estados entre as instâncias de classes de contexto, caso contrário pode trabalhar com variáveis static diretamente nas classes de contexto ou até melhor, utilizar o padrão Singleton nas classes de estado
 
 #Applicability
  - A abordagem baseada em padrões usa código (em vez de estruturas de dados) para especificar transições de estado, mas faz um bom trabalho de acomodar ações de transição de estado.
  - Código visivelmente mais intuitivo e limpo, permitindo fácil evolução e manutenção;
  - A inclusão de um novo estado tende a não quebrar os princípios de orientação a objetos, além de permitir o código evoluir por adição e não por alteração.
  
  #Structure 
  
  ![](https://i2.wp.com/www.devmedia.com.br/imagens/articles/208953/state1.PNG)
  
  #Participants
  
   -Contexto: define a interface com o cliente e mantém a instância de estado concreto o qual define o estado atual do objeto.
   
   -Estado: Interface que permite encapsular as responsabilidades associadas ao estado particular de contexto.
   
   -EstadoConcreto: Um ou mais estados concretos que implementam a interface estado.
   
  #Sample Code 
  
  (https://github.com/charlyandrei/PadraodeProjeto/tree/master/Padrao%20State/CodeState)
