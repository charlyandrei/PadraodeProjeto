# Padrão Projeto Strategy
# Pattern Name and Classification
- Padrão Strategy ou Policy
- Padrão Comportamental

# Intent
  - O objetivo é representar uma operação a ser realizada sobre os elementos de uma estrutura de objetos. O padrão Strategy permite definir novas operações sem alterar as classes dos elementos sobre os quais opera.
  - Strategy permite que o algoritmo varie independentemente dos clientes que o utilizam.
  
# Motivation
  
  - É a melhoria da manutenção do código o qual é frequentemente usado durante o desenvolvimento de uma aplicação. Para tanto, há a necessidade de definir um conjunto de classes para que possam ser alteradas em tempo de execução. Assim os objetos trabalham de forma independente para os possíveis clientes realizarem operações diferentes, sem a dependência de implementação do comportamento de outra classe.
 
 # Applicability
  - O padrão é aplicado em situações em que muitas classes se relacionam e diferem apenas no modo de atuação, com isso o Strategy irá configurar a classe que tenha um dentre muitos comportamentos fornecidos. Outra situação oportuna para o uso do padrão é em uma aplicação na qual se tem um cliente e este não pode ficar exposto a estrutura de dados do algoritmo.
  
  # Structure 
  
  ![](https://i1.wp.com/videos.web-03.net/artigos/Higor_Medeiros/PadraoStrategy/PadraoStrategy1.jpg)
  
  # Participants
  
   -Strategy: É uma interface comum para todas as subclasses, ou para todos os algoritmos que são suportados. O Contexto usa essa interface para chamar uma das subclasses ConcreteStrategy ou um dos algoritmos definidos.
   
   -ConcreteStrategy: A classe concreta que herda da Strategy abstrata está definida como as subclasses ConcreteStrategyA, ConcreteStrategyB e ConcreteStrategyA no diagrama da figura.
   
   -Context: É aquele que vai acessar um dos algoritmos das subclasses de interface Strategy.
   
  # Sample Code 
  
  (https://github.com/charlyandrei/PadraodeProjeto/tree/master/Padrao%20State/CodeState)
