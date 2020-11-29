# Pattern Name and Classification

- Abstract Factory é um padrão de projeto de software

# Intent
  - O uso deste padrão torna possível trocar implementações concretas sem alterar o código que estas usam, mesmo em tempo de execução. No entanto, o emprego deste padrão, como acontece com outros padrões semelhantes, pode resultar em uma complexidade desnecessária e trabalho extra no início do código. A essência do padrão Abstract Factory é fornecer uma interface para criar famílias de objetos relacionados ou dependentes sem especificar suas classes concretas

# Motivation
  - É útil para fornecer uma interface para criar famílias de objetos relacionados ou dependentes sem especificar suas classes concretas, a criação de objetos de seu uso e criar famílias de objetos relacionados sem ter que depender de suas classes concretas. Isto permite novos tipos derivados de ser introduzidas sem qualquer alteração ao código que usa a classe base .

# Applicability
  - A fábrica determina o tipo concreto do objeto a ser criado, e é nela que o objeto é realmente criado. No entanto, a fábrica só retorna um ponteiro abstrato para o objeto concreto criado.O código do cliente não tem conhecimento algum do tipo concreto. Objetos concretos são, de fato criados pela fábrica, mas o código do cliente acessa tais objetos só através da sua interface abstrata.A adição de novos tipos concretos é feita modificando o código do cliente para usar uma fábrica diferente, uma modificação que é tipicamente uma linha em um arquivo. A nova fábrica, em seguida, cria objetos de um tipo de concreto diferente, mas ainda retorna um ponteiro do mesmo tipo abstrato como antes.
  
  # Structure 
  
  ![](https://upload.wikimedia.org/wikipedia/commons/thumb/4/4c/Abstract_Factory.png/556px-Abstract_Factory.png)
  
  # Participants
  
- WidgetFactory
- MotifWidgetFactory
- QtWidgetFactory
- Cliente
- Botao
- BotaoQt
- BotaoMotif
- Janela
- JanelaMotif
- JanelaQt
   
  # Sample Code 
  
  (https://github.com/charlyandrei/PadraodeProjeto/tree/master/Padrao%20State/CodeState)
