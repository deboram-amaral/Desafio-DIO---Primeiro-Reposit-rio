# Lógica de Programação Essencial :desktop_computer:

* Após o entendimento teórico de alguns conceitos chave, no segundo momento do conteúdo entramos na linguagem do Portugol!

### O que são linguagens de programação?

* "Linguagem escrita e formal que especifica um conkinto de instruções e regras usadas para gerar programas (Softwares). Um software pode ser desenvolvido para rodar em um computador, dispositivo mível ou em qualquer equipamento que permita sua execução."

  * Meio de comunicação entre computadores e humanos!

  

  As linguagens de programação podem ser de Alto nível (se aproximam mais da nossa linguagem, mais polida) ou de Baixo nível (mais rudimentares como arquitetura de rádio). Além disso, podem ser:

  * Compiladas
    Linguagem de programação em que o código fonte, é executado diretamente pelo sistema operacional ou pelo processador, após ser traduzido por meio de um processo chamado compilação.
  * Interpretadas
    Linguagens de programação em que o código fonte é executado por um programa de computador chamado interpretador que em seguida é executado pelo sistema operacional ou processador
    Ex.: Java, PHP...



## Portugol

* Pseudolinguagem mais utilizada!

* Alguns comandos

  | Quebra de linha                              | "\n"         |
  | -------------------------------------------- | ------------ |
  | Escrever comentário sem interferir no código | //comentário |
  | Adicionar um                                 | ++           |

  

  ### Desvios condicionais e laços de repetição

  

  * Desvio condicional - SE
    É utilizada a palavra reservada SE, a condição a ser testada entre parenteses e as instruções que devem ser executadas entre chaves caso o desvio seja verdadeiro:

    

    **SE(media>=7) {**

    ​				**escreva ("Parabéns, você foi aprovado!")**

    **}**

    ​				**SENAO {**

    ​							**escreva ("Infelizmente você foi reprovado.")**

    ​			**}**

    

  * **Desvio condicional - CASO**

    *"Comando similar aos comandos SE e SENAO, reduz a complexidade na escolha de diversas opções. Apesar das similaridades com o SE, possui algumas diferenças. Neste comando não é possível o uso de operadores lógicos, ele apenas trabalha com valores definidos."*

  * **Laços de repetição em Portugol**
    *"Dentro da lógica de programação, é uma estrutura que permite executar mais de uma vez o mesmo comando ou conjunto de comandos, de acordo com uma condição ou com um contador"*

    

    **Função início ()**

    **{**

    ​		**INTEIRO contador, limite, resultado**
    ​		**contador = 0**
    ​		**limite = 10**

    ****

    ​		**FACA**
    ​		**{**

    ​					**resultado = 9*contador**
    ​					**escreva ("9x" + contador + "=" + resultado + ""\n")**
    ​					**contador++**

    ​		**} enquanto (contador<=limite)**

    **}**

  

  ### Matrizes e vetores

  * **Matriz**
    *" Coleção de variáveis de **mesmo tipo**, acessíveis com um único nome e armazenados contiguamente na memória."*

    **Sequência de variáveis!** Possuem mais de uma dimensão. Ex.: colunas e linhas.

    *" A individualização de cada variável de um vetor é feita atravez do uso de índices"*

  * **Vetor**
    Os vetores são matrizes de uma só dimensão. Ex.: só colunas.
    Exemplo mais prático:

    

    CADEIA vetor[5] //declara um vetor de 5 posições

    CADEIA matriz [5] [3] // declara uma matriz de 5 linhas e 3 colunas

    

    CADEIRA frutas [4]

    frutas[0] = "Maçã"
    frutas[1] = "Pêra"
    frutas[2] = "Uva"
    frutas[3] = "Melão"

    //índice sempre inicial por 0

    escreva (frutas[2]) //será devolvido "Uva"

    

    CADEIRA cesta [] [] = {{"Maçã", "100"}, {"Pêra", "200"}, {"Melão", "300"}}

    escreva "Fruta: " + cesta [0] [] + "Quantidade: " + cesta [0] [1] + "\n"

    //será devolvido
    Fruta: Maça  Quantidade: 100
    Fruta: Pêra  Quantidade: 200
    Fruta: Melão  Quantidade: 300

    

