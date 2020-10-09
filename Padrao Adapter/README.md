# Padrão Projeto Adapter
1.Pattern Name and Classification
Essa implementação usa o princípio de composição do objeto: o adaptador implementa a interface de um objeto e encobre o outro. Ele pode ser implementado em todas as linguagens de programação populares.
  -Intent
  O Adapter é um padrão de projeto estrutural que permite objetos com interfaces incompatíveis colaborarem entre si.
  Você pode criar um adaptador. Ele é um objeto especial que converte a interface de um objeto para que outro objeto possa entendê-lo
  - Motivation
    Imagine que você está criando uma aplicação de monitoramento do mercado de ações da bolsa. A aplicação baixa os dados as ações de múltiplas fontes em formato XML e então mostra gráficos e diagramas maneiros para o usuário.
Em algum ponto, você decide melhorar a aplicação ao integrar uma biblioteca de análise de terceiros. Mas aqui está a pegadinha: a biblioteca só trabalha com dados em formato JSON.
Você poderia mudar a biblioteca para que ela funcione com XML. Contudo, isso pode quebrar algum código existente que depende da biblioteca. E pior, você pode não ter acesso ao código fonte da biblioteca para começo de conversa, fazendo dessa abordagem uma tarefa impossível.  
  - Applicability
     Utilize a classe Adaptador quando você quer usar uma classe existente, mas sua interface não for compatível com o resto do seu código.
  
  -![Structure](https://refactoring.guru/images/patterns/diagrams/adapter/example.png)
  
  - Participants
  
   -Target define a interface específica do domínio que o Cliente usa.
   
   -Adapter adapta a interface Adaptee à interface de destino.
   
   -Adaptee define uma interface existente que precisa de adaptação.
   
   -Client colabora com objetos em conformidade com a interface de destino.
  -[] Sample Code ()
