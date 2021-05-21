<br>
<p align="center">
  <a href="https://www.uminho.pt" target="_blank"><img src="https://i.imgur.com/FXQo8OL.png" alt="Universidade do Minho"></a>
  <a href="https://www.eng.uminho.pt" target="_blank"><img src="https://i.imgur.com/WABo4st.png" alt="Escola de Engenharia"></a>
  <br><a href="http://www.dsi.uminho.pt" target="_blank"><strong>Departamento de Sistemas de Informação</strong></a>
  
  <h2 align="center">Projeto Prático SBC - MIEGSI 2020/2021</h2>
  <br>
  
## Índice de conteúdos

- [Índice de conteúdos](#índice-de-conteúdos)
- [Introdução <a name = "intro"></a>](#introdução-)
- [Tarefa A - Aconselhamento para compra de uma refeição <a name = "ta"></a>](#tarefa-a---aconselhamento-para-compra-de-uma-refeição-)
  - [Parte 1 - Aquisição manual de conhecimento  <a name = "ta1"></a>](#parte-1---aquisição-manual-de-conhecimento--)
  - [Parte 2 - Aquisição automática de conhecimento <a name = "ta2"></a>](#parte-2---aquisição-automática-de-conhecimento-)
  - [Pré-requisitos <a name = "pre1"></a>](#pré-requisitos-)
- [Getting started <a name = "getting1"></a>](#getting-started-)
  - [Quick-start <a name = "quick1"></a>](#quick-start-)
    - [Start your application ....](#start-your-application-)
  - [Installation  <a name = "install1"></a>](#installation--)
    - [Add SWI-Prolog to the PATH environment variable](#add-swi-prolog-to-the-path-environment-variable)
    - [Clone the repo](#clone-the-repo)
    - [Install all the dependecies](#install-all-the-dependecies)
  - [Usage  <a name = "usage1"></a>](#usage--)
- [Tarefa B - Aconselhamento de trajeto para entrega de uma refeição <a name = "tb"></a>](#tarefa-b---aconselhamento-de-trajeto-para-entrega-de-uma-refeição-)
  - [Parte 1 - Resolução via Procura <a name = "tb1"></a>](#parte-1---resolução-via-procura-)
  - [Parte 2 - Otimização do lucro, tempo ou ambos <a name = "tb2"></a>](#parte-2---otimização-do-lucro-tempo-ou-ambos-)
  - [Pré-requisitos <a name = "pre2"></a>](#pré-requisitos--1)
- [Getting started <a name = "getting2"></a>](#getting-started--1)
  - [Quick-start <a name = "quick2"></a>](#quick-start--1)
    - [Clone the repo](#clone-the-repo-1)
  - [Usage <a name = "usage2"></a>](#usage-)
- [Ferramentas <a name = "built"></a>](#ferramentas-)
- [Contactos <a name = "contact"></a>](#contactos-)
- [Acknowledgments <a name = "ack"></a>](#acknowledgments-)
- [Referências <a name = "refer"></a>](#referências-)
- [Licensa <a name = "license"></a>](#licensa-)

## Introdução <a name = "intro"></a>

No âmbito da unidade curricular de Sistemas Baseados em Conhecimento, foi-nos proposto a conceção de um SBC implementado na linguagem Prolog, estando a mesma dividida em 2 tarefas com 2 partes cada uma, tendo por base o conceito de food delivery, tão em voga no último ano decorrente da situação pandémica que vivenciamos.


## Tarefa A - Aconselhamento para compra de uma refeição <a name = "ta"></a>
Tem o objetivo de desenvolver um sistema baseado em conhecimento, utilizando a linguagem Prolog, de modo a aconselhar um menu específico ao utilizador com um conjunto de refeição que pode pedir.

### Parte 1 - Aquisição manual de conhecimento  <a name = "ta1"></a>
Inicialmente, foi desenvolvida uma pesquisa com o intuito de reunir uma lista de pratos diversificada, que respeitassem as diferentes preferências dos utilizadores. 
Com base neste conhecimento, foi desenvolvido o ficehiro "pratos.pl" (base de conhecimento) com um conjunto de regras de produção, em Prolog, com as combinações possíveis, com o formato: “if X and Y and Z and W then ‘menu’”, na qual “menu” consiste num conjunto de refeições sugeridas. 
Os parâmetros X, Y, Z, W correspondem às escolhas que cada utilizador fará ao responder às questões apresentadas na interface.
A base de dados foi criada no ficheiro "bd.pl" que agrega os diferentes menus, com os respetivos pratos associados. 
O sistema de inferência utilizado foi o Forward Chaining, que com base nos factos representados na base de conhecimento, o raciocínio avança na rede de inferência até obter uma resposta, atribuindo um menu a um utilizador. 


### Parte 2 - Aquisição automática de conhecimento <a name = "ta2"></a>
Na segunda parte, foi desenvolvido um questionário a utilizadores, com o objetivo de reunir um conjunto alergado de respostas sobre as preferências de cada um. 
Com base no ficheiro "questionarioSBC.csv" e recorendo à ferramenta Weka, foi possível ao grupo adquirir conhecimento de forma automática, uma vez que o Weka produz um conjunto de regras a partir do csv..
O ficheiro "pratos.pl" contém as novas regras de produção retiradas da ferramenta e todos os restantes ficheiros utilizados são em tudo semelhantes aos da primeira parte desta tarefa.


### Pré-requisitos <a name = "pre1"></a>
* [SWI-Prolog 8.2.4](https://www.swi-prolog.org/download/stable)
* [Weka](https://waikato.github.io/weka-wiki/downloading_weka/)
* Outros......


## Getting started <a name = "getting1"></a>

### Quick-start <a name = "quick1"></a>

#### Start your application ....
  ```run .....
  ```

### Installation  <a name = "install1"></a>
#### Add SWI-Prolog to the PATH environment variable
#### Clone the repo
  ```sh
  git clone https://github.com/flsantana00/SBC.git
  ```
#### Install all the dependecies
  ```sh
  xxxxxx
  ```

### Usage  <a name = "usage1"></a>


## Tarefa B - Aconselhamento de trajeto para entrega de uma refeição <a name = "tb"></a>
A tarefa B tem como objetivo o desenvolvimento de um sistema baseado em conhecimento, que auxilia o trabalho de um estafeta que utiliza uma scooter para entregar refeições de um restaurante.

Desenvolver um SBC para um estafeta que usa uma scooter como meio de transporte que trabalha para um sistema de entrega de um restaurante. O SBC deve aconselhar que encomendas o estafeta deve pegar no restaurante e qual o caminho a seguir para proceder às entregas. Optamos por desenvolver xxxx.

### Parte 1 - Resolução via Procura <a name = "tb1"></a>
A primeira parte desta tarefa encontra-se dividida em dois objetivos distintos. No primeiro, o sistema gera de forma random um cliente e apresenta os caminhos possíveis para tal. No segundo, o sistema gera de forma random dois clientes e o sistema apresenta os caminhos possíveis para a entrega.
Em ambos os objetivos o estafeta pode consultar o tempo e lucro associado a cada caminho apresentado.
No ficheiro "bd2.pl", inicialmente, define-se o goal dinamicamente, através da regra def_goal(X,Client), consoante o cliente random gerada na interface.
Posteriormente, são declarados os diferentes arcos entre os clientes e entre o restaurante, assim como as durações e os lucros associados a cada percurso. 
Em seguida, são definidas regras que permitem ao sistema calcular o tempo (tempo([Cliente1,Cliente2|R],DS)) e o lucro (valor(ClienteF,VS)) de cada caminho apresentado ao estafeta, assim como um regra que permite avançar de cliente em cliente, ao longo do grafo, s(N1,N2). 
Por fim, encontra-se uma regra que invoca o sistema de inferência que realiza a procura (run(Method,S,V,T)), sendo o ficheiro "search.pl" fornecido pelo professor Paulo Cortez e que permite executar os métodos de pesquisa breadthfirst e o depthfirst, que se encontram nos ficheiros "detphfirst.pl" e "breathfisrt.pl".
 
    
De forma similar, o grupo desenvolveu o ficheiro "bdObjetivo2.pl", em que dinamicamente é definido o goal dos dois clientes gerados de forma random (goal(X)). 
Posteriormente, são declarados igualmente os diferentes arcos entre os clientes e entre o restaurante, assim como as durações e os lucros associados a cada percurso. 
Em seguida, foram definidas regras que permitem ao sistema calcular o tempo (tempo([Cliente1,Cliente2|R],DS)) e o lucro (valor(VS)) de cada caminho apresentado ao estafeta, assim como um regra que permite avançar de cliente em cliente, ao longo do grafo, s(N1,N2). 
Por fim, encontra-se regra que invoca o sistema de inferência que realiza a procura (run(Method,LS,V,T)), sendo o ficheiro "search.pl" fornecido pelo professor Paulo Cortez e que permite executar os métodos de pesquisa breadthfirst e o depthfirst, que se encontram nos ficheiros "detphfirst.pl" e "breathfisrt.pl".


Nesta parte foram desenvolvidas as funcionalidades de procura para o objetivo 1 

### Parte 2 - Otimização do lucro, tempo ou ambos <a name = "tb2"></a>
Nesta parte foram desenvolvidas as funcionalidades de optimização usando o método de hillclimbing para o objetivo A (maximizar o lucro), B (minimizar o tempo do percurso) e C (maximizar 0.8*lucro+0.2*(20-tempo)).XXXXXX


### Pré-requisitos <a name = "pre2"></a>
* [Liste aqui]

### Tarefa Desenvolvido por: <a name = "equipa=></a>
Ana Paula Martins a89196 
   
Ana Miguel Roseta a89209 
 
Catarina Fernandes a89206
   
Francisca Santana a89225

## Getting started <a name = "getting2"></a>

### Quick-start <a name = "quick2"></a>

#### Clone the repo
  ```sh
  git clone https://github.com/flsantana00/SBC.git
  ```

### Usage <a name = "usage2"></a>


  
## Ferramentas <a name = "built"></a>
* [SWI-Prolog](https://www.swi-prolog.org)



## Contactos <a name = "contact"></a>

* [EU](mailto:eu0@hotmail.com)
* [Tu](mailto:tu@gmail.com)
* [Vos](mailto:vos@gmail.com)


## Acknowledgments <a name = "ack"></a>
* [Paulo Cortez](http://www3.dsi.uminho.pt/pcortez/Home.html)
* [André Pilastri](https://pilastri.github.io/andrepilastri.github.io/#about)

## Referências <a name = "refer"></a>

## Licensa <a name = "license"></a>

Distributed under the MIT License. See `LICENSE` for more information.
