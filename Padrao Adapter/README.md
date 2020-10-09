# Padrão Projeto Adapter
1.Pattern Name and Classification
Essa implementação usa o princípio de composição do objeto: o adaptador implementa a interface de um objeto e encobre o outro. Ele pode ser implementado em todas as linguagens de programação populares.
  -Intent
  O Adapter é um padrão de projeto estrutural que permite objetos com interfaces incompatíveis colaborarem entre si.
  Você pode criar um adaptador. Ele é um objeto especial que converte a interface de um objeto para que outro objeto possa entendê-lo
  - Motivation
  
    O padrão do adapter está se adaptando entre classes e objetos. Como qualquer adaptador no mundo real, ele é usado para ser uma interface, uma ponte entre dois objetos. No mundo real, temos adaptadores para fontes de alimentação, adaptadores para cartões de memória de câmera e assim por diante. Provavelmente todo mundo viu alguns adaptadores para cartões de memória. Se você não pode conectar a memória da câmera em seu laptop, você pode usar um adaptador. Você conecta a memória da câmera no adaptador e o adaptador no slot do laptop. É isso, é muito simples.
  - Applicability
     Utilize a classe Adaptador quando você quer usar uma classe existente, mas sua interface não for compatível com o resto do seu código.
  
  - Structure 
  
  ![](https://refactoring.guru/images/patterns/diagrams/adapter/example.png)
  
  - Participants
  
   -Target define a interface específica do domínio que o Cliente usa.
   
   -Adapter adapta a interface Adaptee à interface de destino.
   
   -Adaptee define uma interface existente que precisa de adaptação.
   
   -Client colabora com objetos em conformidade com a interface de destino.
  -[] Sample Code ()
