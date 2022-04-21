# Aprenda o que são Estruturas de Dados e Algoritmos :computer:



### 1 - Conceitos iniciais sobre estrutura de dados, arrays e registros

* O que é estrutura de dados?

  * Estrutura de dados é uma estrutura organizada de dados na memória de um computador ou em qualquer dispositivo de armazenamento, de forma que os dados possam ser utilizados de forma correta
    * As estruturas de dados encontram complicações no desenvolvimento de sistemas. Usando as estruturas adequadas através de algoritmos, é possível trabalhar com uma grande quantidade de dados.
  * O que são algoritmos?
    * Conjunto de instruções estruturadas e ordenadas para realizar operação específica. Sâo utilizados para manipular dados nas estruturas de várias formas: **inserir, excluir, procurar e ordenar dados.**
  * Em uma estrutura de dados devemos saber como realizar um determinado conjunto de operações básicas como:
    * Inserir dados;
    * Excluir dados;
    * Localizar um elemento;
    * Percorrer todos os itens da estrutura para sua visualização;
    * Classificar (colocar os itens de dados em uma determinada ordem. Ex.: numérica, alfabética etc).
  * Principais estruturas de dados:
    * Vetores e matrizes;
    * Registros;
    * Listas;
    * Pilhas;
    * Filas;
    * Árvores;
    * Tabelas Hash;
    * Grafos.

* Vetores e Matrizes (Arrays)
  * Estrutura de dados simples que podem auxiliar quando há muitas variáveis do mesmo tipo em um algoritmo.
  * VETORES
    * Vetor ou **Array Uni-dimensional** é uma variável que armazena várias variáveis do mesmo tipo;
    * O Vetor é uma estrutura de dados indexada, que pode armazenar uma determinada quantidade de valores do mesmo tipo.
  * MATRIZES
    * Matriz ou **Array Multi-dimensional** é um vetor de vetores;
    * Uma matriz é um vetor que possui duas ou mais dimensões. Ex.: linhas e colunas.
* Registros
  * Registro é uma estrutura de dados que fornece um formato especializado para armazenar informações em memória.
  * Enquanto arrays nos permite armazenar vários dados de um único tipo de dados, o recurso Registro nos permite armazenar mais de um tipo de dados. Ex.: Cadastro de funcionário com nome, CPF, endereço e contato (caracteres, alfanúmeros...)
  * Toda estrutura de registro tem um nome e seus campos podem ser acessados por meio do uso do operador ponto **(.)**. Exemplo: registro livro. Para acessar o preço de um livro, poderíamos utilizar: **livro.preco**.



### 2- Entenda o que são Listas, Pilhas e Filas

* O que são listas

  * Estruturas de dados do tipo lista armazenam dados de um determinado tipo em uma ordem específica;

  * As listas possuem tamanhos ajustáveis enquanto arrays possuem tamanhos fixos. Isso quer dizer que sempre vai existir a possibilidade da lista aumentar, ser composta por novos dados;

  * Existem dois tipos de listas:

    * Ligadas: na estrutura do tipo lista existem os **nós** em que cada um conhece o valor que está sendo armazenado em seu interior, além de conhecer o elemento posterior a ele: por isso ela é chamada de "Lista ligada", pois os nós são amarrados com essa indicação de qual é o próximo nó.
      ![](C:\Users\debor\OneDrive\Imagens\ListaEncadeada.jpg)

      

    * Duplamente ligadas: Constituem uma variação das listas ligadas. A diferença é que listas duplamente ligadas são **bidirecionais**. Os nós sabem qual é o próximo elemento e também o anterior.
      ![](C:\Users\debor\OneDrive\Imagens\Captura de tela de 2015-08-11 15_02_34.png)



* O que são pilhas 
  * Estruturas de dados que servem como uma coleção de elementos e permitem o acesso a somente um item de dados armazenados.
  * O acesso aos itens de uma pilha é restrito - somente um item pode ser lido ou removido por vez.
  * Há dois tipos de pilhas:
    * Pilha LIFO (Last in First Out) / UESP (Último que entra, primeiro que sai)
      Apresenta o seguinte critério: o primeiro elemento a ser retirado é o último que tiver sido inserido.
      ![](C:\Users\debor\OneDrive\Imagens\Lifo_stack.svg.png)
    * Pilha FIFO (First in First Out) / PEPS (Primeiro que entra, primeiro que sai)
      Apresenta o seguinte critério: o primeiro elemento a ser retirado é o primeiro que tiver sido inserido.
      ![](C:\Users\debor\OneDrive\Imagens\Fifo_queue.png)



* O que são Filas
  * A estrutura de dados do tipo Fila admite remoção de elementos e inserção de novos sujeita à seguinte regra de operação: o elemento removido é o que está na estrutura há mais tempo. Ou seja: o primeiro a ser removido, seguindo o conceito FIFO.



### 3 - Estruturas de dados do tipo Árvore, Tabela Hash e Grafos

* O que são árvores
  * Árvore é uma estrutura de dados que organiza seus elementos de forma hierárquica, onde existe um elemento que fica no topo da árvore, chamado de **raiz** e existem elementos subordinados a ele, que são chamados de **nós** ou **folhas**. 
    ![](C:\Users\debor\OneDrive\Imagens\Arvore_05.png)



* O que são Tabelas Hash
  * Uma Tabela Hash, de dispersão ou espalhamento, é uma estrutura de dados especial, que associa chaves de pesquisa a valores.
  * É uma generalização da ideia de array. Porém utiliza uma função denominada Hashing para espalhar os elementos, fazendo com que os mesmos fiquem de forma não ordenada dentro do "array" que define a tabela.
  * Por que espalhar?
    * A tabela hash permite a associação de "valores" a "chaves".
    * Valores: é a posição ou índice onde o elemento se encontra.
    * Chave: parte da informação que compõe o elemento a ser manipulado.
    * Espalhar facilita a busca na estrutura de dados, pois a partir de uma chave, podemos acessar de uma forma rápida uma posição do array.
      ![](C:\Users\debor\OneDrive\Imagens\tabela hash.webp)



* O que são Grafos
  * Grafos são estruturas que permitem programar a relação entre objetos. Os objetos são variáveis ou "nós" do grafo. Os relacionamentos são arestas.
    Exemplo de codificação de grafos: redes sociais, linhas de ônibus...
    ![](C:\Users\debor\OneDrive\Imagens\fr.png)