# Pattern Name and Classification
- Padrão Template Method
- Padrão Comportamental

# Intent
  - Definir o esqueleto de um algoritmo
  - Definir um algoritmo usando operações abstrata
  
# Motivation
  
  - Application Framework para editores de documentos
  
 # Applicability
  - Para implementar partes invariantes de um algoritmo uma única vez
  - Quando comportamento comum entre subclasses deveria ser fatorado e localizado numa classe comum para evitar duplicação
  - Controlar extensões de subclasses
  
  # Structure 
  
  ![](https://padroesdeprojetoifc.files.wordpress.com/2016/11/templatemethod1.gif?w=616)
  
  # Participants
  
## ClasseAbstrata (Login)
- Define operações abstratas que subclasses concretas definem para implementar certas etapas do algoritmo
- Implementa um Template Method definindo o esqueleto de um algoritmo
- O Template Method chama várias operações, entre as quais as operações abstratas da classe
   
## ClasseConcreta (LoginDecisionSupportSystem)
-Implementa as operações abstratas para desempenhar as etapas do algoritmo que tenham comportamento específico a esta subclasse
     
  # Sample Code 
  
  (https://github.com/charlyandrei/PadraodeProjeto/tree/master/Padrao%20Singleton/codeSingleton)
