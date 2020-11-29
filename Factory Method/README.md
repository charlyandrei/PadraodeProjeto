# Pattern Name and Classification
- Factory Method 
- Padrão de Criação.

# Intent
  - Definir uma interface para criar objetos de forma a deixar subclasses decidirem qual classe instanciar;
  - Factory Method deixa que subclasses façam a instanciação.
  
# Motivation
  
  - Não precisa conhecer a classe para retornar uma opção dela através de um método.
  
 # Applicability
  - Quando uma classe (o criador) não pode antecipar a classe dos objetos que deve criar;
  - Quando uma classe quer que suas subclasses especifiquem os objetos criados;
  - Quando classes delegam responsabilidade para uma entre várias subclasses de apoio e queremos localizar num ponto único a conhecimento de qual subclasse está sendo usada.
  
  # Structure 
  
  ![](https://padroesdeprojetoifc.files.wordpress.com/2016/11/factory1.gif?w=616)
  
  # Participants
  
- Criador: declara o Factory Method que retorna um objeto do tipo Produto;
Às vezes, o Criador não é apenas uma interface mas pode envolver uma classe concreta que tenha uma implementação default para o Factory Method para retornar um objeto com algum tipo ProdutoConcreto default;
Pode chamar o Factory Method para criar um produto do tipo Produto;

- CriadorConcreto: faz override do Factory Method para retornar uma instância de ProdutoConcreto;

- Produto: define a interface dos objetos criados pelo Factory Method;

- Produto Concreto: implementa a interface Produto.
   
  # Sample Code 
  
  (https://github.com/charlyandrei/PadraodeProjeto/tree/master/Padrao%20State/CodeState)
