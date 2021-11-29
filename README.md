# Deep Cars

Projeto onde várias Redes Neurais competem para aprender a dirigir em uma pista de corrida com obstáculos.

![Preview-Screens](https://github.com/JVictorDias/DeepCars/blob/master/preview.gif)

# Sobre o Projeto

  A ideia consiste em utilizar uma "seleção artificial" para evoluir os pesos de várias redes neurais, com o propósito de encontrar a melhor combinação e assim obter o melhor comportamento para os carros.
  
  O simulador foi criado do zero(sem engines) utilizando a biblioteca gráfica **Programming Interface Gaming (PIG)** que por sua vez é baseada na tradicional **Simple DirectMedia Layer (SDL)**.
  
  A Rede Neural Artificial utilizada foi uma Perceptron Multilayer com 3 camadas!

  - Camada de Entrada com 18 sensores + 1 Viés, totalizando 19 Neurônios
  - Camada Escondida com 6 neurônios + 1 Viés, totalizando 7 Neurônios
  - Camada de Saída com 4 neurônios (Acelerar, Ré, Virar para a Esquerda, Virar para a Direita)
  - A função de ativação utilizada em todos os neurônios foi a ReLU.
  - O método de aprendizagem é comumente chamado de "Random Mutations".
  - O tamanho da população que utilizei foi de 1000 indivíduos.
  - O tempo de aprendizagem variou entre 5 ~ 20 minutos.

# Por quê?
Trabalho requisitado pela professora Andressa da disciplina de Inteligência Artificial e Computacional como requisito avaliativo do bimestre. 
### Produzido por: Daniel Queiroz e Rafael Buchacra
# Observações:

- O arquivo 'redeNeural.c' contém todas as funções relativas à implementação da Rede Neural (tudo sobre a rede neural está nesse arquivo).
 
 Exemplo:
    ```
    RedeNeural* Car = RNA_CriarRedeNeural(1,2,3,4);
    ```          
    Nesse exemplo nós estamos criando uma variável chamada 'Car' que vai receber a Rede Neural que foi alocada dentro da função RNA_CriarRedeNeural()... 
    Utilizando a  função
    ```
    RNA_DestruirRedeNeural(Car);
     ```      
- A função 'ControlarEstadoCarros' dentro do arquivo 'main.cpp' contém o código que faz a comunicação entre o simulador e a rede neural.
- O resto dos arquivos são apenas os códigos da implementação do simulador.

