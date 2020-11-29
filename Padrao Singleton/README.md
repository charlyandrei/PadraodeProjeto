# Padrão Projeto Singleton
# Pattern Name and Classification
- Padrão Singleton
- Padrão Criacional

# Intent
  - Assegurar que uma classe tenha uma única instância e prover um ponto de acesso global a esta instância.
  
# Motivation
  
  - Algumas classes devem ser instanciadas uma única vez;
  - Um spooler de impressão;
  - Um gerenciador de janelas;
  - Um objeto que contém a configuração de um programa.
  
 # Applicability
  - Deve haver uma única instância de uma classe e esta instância deve ser acessada a partir de um ponto de acesso bem-conhecido;
  - Quando a instância única deve ser extensível através de subclasses e clientes podem usar instâncias diferentes polimorficamente, sem modificação de código.
  
  # Structure 
  
  ![](https://miro.medium.com/max/403/1*m8oZpTQqTFnjLAgdQORb_g.png)
  
  # Participants
  
   -Singleton: O construtor é privado, não sendo acessível externamente.
   
   -getInstance(): , que retorna a instância privada do objeto singleton da classe.
   
   
  # Sample Code 
  
  (https://github.com/charlyandrei/PadraodeProjeto/tree/master/Padrao%20State/CodeState)
