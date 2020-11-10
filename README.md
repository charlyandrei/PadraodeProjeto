# Padrão Projeto Adapter
1.Pattern Name and Classification

Essa implementação usa o princípio de composição do objeto: o adaptador implementa a interface de um objeto e encobre o outro. Ele pode ser implementado em todas as linguagens de programação populares.
 
 -Intent
  É um padrão de design comportamental que permite salvar e restaurar o estado anterior de um objeto sem revelar os detalhes de sua implementação.
  
  - Motivation
  
   Às vezes, é necessário capturar o estado interno de um objeto em algum ponto e ter a capacidade de restaurar o objeto a esse estado posteriormente. Tal caso é útil em caso de erro ou falha. Considere o caso de um objeto calculadora com uma operação desfazer, tal calculadora poderia simplesmente manter uma lista de todas as operações anteriores que executou e, portanto, seria capaz de restaurar um cálculo anterior que executou. Isso faria com que o objeto calculadora se tornasse maior, mais complexo e pesado, já que o objeto calculadora teria que fornecer funcionalidade de desfazer adicional e manter uma lista de todas as operações anteriores. Esta funcionalidade pode ser removida da classe da calculadora, de forma que uma classe externa (vamos chamá-la de classe de gerenciador de desfazer) pode coletar o estado interno da calculadora e salvá-lo.
   
  - Applicability
    Um zelador gostaria de realizar uma operação no Originador enquanto tem a possibilidade de reverter. O caretaker chama o método createMemento () no originador, pedindo ao originador para passar um objeto memento. Neste ponto, o originador cria um objeto memento salvando seu estado interno e passa o memento para o zelador. O zelador mantém o objeto memento e executa a operação. No caso de necessidade de desfazer a operação, o zelador chama o método setMemento () no originador passando o objeto memento mantido. O originador aceitaria o memento, usando-o para restaurar seu estado anterior.
  
  - Structure 
  
  ![](https://www.oodesign.com/images/design_patterns/structural/memento-design-pattern-implementation-uml-class-diagram.png)
  
  - Participants
  
   -Memento Armazena o estado interno do objeto Originador. O estado pode incluir qualquer número de variáveis ​​de estado.
O Memento deve ter duas interfaces, uma interface para o zelador. Esta interface não deve permitir nenhuma operação ou qualquer acesso ao estado interno armazenado pelo memento e, portanto, honra o encapsulamento. A outra interface é para o originador e permite que o originador acesse quaisquer variáveis ​​de estado necessárias para que o originador restaure o estado anterior
   
   -Originator Cria um objeto memento capturando o estado interno do originador.
Use o objeto memento para restaurar seu estado anterior.
   
   -Caretaker Responsável por guardar o memento.
O memento é opaco para o zelador, e o zelador não deve operá-lo
   
  - Sample Code 
  
  (https://github.com/charlyandrei/PadraodeProjeto/blob/master/Padrao%20Adapter/CodeAdapter)
