# Padrão Projeto Composite
# Pattern Name and Classification
- Padrão Estrutural

# Intent
  - Reutilizar método e funções de algum objeto;
  - Transferir para outro qualquer;
  - Sendo vários objetos ligados a um único.
  
# Motivation
  
  - Em certas estruturas necessitamos por muitas vezes de métodos e funções que já estão especificadas em um determinado objeto, sendo necessário apenas a ligação entre os dois para assim poder ser reutilizado o código.

 # Applicability
  - Construir objetos existindo objetos do mesmo tipo.
  
  # Structure 
  
  ![](https://padroesdeprojetoifc.files.wordpress.com/2016/11/800px-composite_uml_class_diagram_fixed-svg.png?w=616)
  
  # Participants
  
#### Component:
- Declara a interface para objetos na  composição;
- Implementa comportamento default para  interface comum a todas as classes, como apropriado;
- Declara uma interface para acessar ou gerenciar seus componentes filhos.
   
#### Leaf: 
- Representa objetos folhas na composição;
- Define comportamento para objetos  primitivos na composição.
- EstadoConcreto: Um ou mais estados concretos que implementam a interface estado.

#### Composit: 
- Define comportamento para Componentes que têm filhos;
- Armazena Componentes filhos;
- implementa operações relacionadas com filhos na interface do Componente

#### Client:
- Manipula objetos na composição através da interface Componente.
   
  # Sample Code 
  
  (https://github.com/charlyandrei/PadraodeProjeto/tree/master/Padrao%20Composite/CodeComposite)
