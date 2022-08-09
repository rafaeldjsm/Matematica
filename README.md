# Matemática
Algumas questões de matemática com soluções analíticas e numéricas.

Simulações Numéricas de problemas interessantes de Matemática e Estatistíca


## [Problema beecrowd Nº 1435 - Matriz Quadrada I](https://github.com/rafaeldjsm/Matematica/blob/main/beecrowd_1435.ipynb)

### Escreva um algoritmo que leia um inteiro N (0 ≤ N ≤ 100), correspondente a ordem de uma matriz M de inteiros, e construa a matriz de acordo com o exemplo abaixo.

> Entrada
>>A entrada consiste de vários inteiros, um valor por linha, correspondentes as ordens das matrizes a serem construídas. O final da entrada é marcado por um valor de ordem igual a zero (0).

> Saída
>> Para cada inteiro da entrada imprima a matriz correspondente, de acordo com o exemplo. Os valores das matrizes devem ser formatados em um campo de tamanho 3 justificados à direita e separados por espaço. Após o último caractere de cada linha da matriz não deve haver espaços em branco. Após a impressão de cada matriz deve ser deixada uma linha em branco.

## [O Problema do rato no labirinto](https://github.com/rafaeldjsm/Matematica/blob/main/caminhoab_90g.ipynb)

>Ajude um rato a encontrar um pedaço de queijo num labirinto como o do desenho da figura 1: Um labirinto desses pode ser representado por uma matriz retangular L, cujo elemento $L[i][j]$ vale 0 ou −1 conforme a casa correspondente do labirinto seja uma passagem livre ou uma parede, respectivamente.
>Suponha que, a cada passo, o rato possa se deslocar de apenas uma casa na vertical ou na horizontal.

<p align="center">
  <img src ='https://raw.githubusercontent.com/rafaeldjsm/Matematica/master/imagens/rato_labirinto.PNG' width=500px></p>

### Saída de Dados 

>A saída do seu programa deve ser uma lista de coordenadas que comece pela posição inicial do rato e termine na posição inicial do queijo. Essa sequencia de coordenadas deve indicar o caminho mais curto para o rato chegar ao queijo.

## [O Problema do rato no labirinto - Caminho Diagonal](https://github.com/rafaeldjsm/Matematica/blob/main/caminhoab_diag.ipynb)

### Neste caso vamos considerar um problema alternativo em que é possível a locomoção nas casas horizontais, verticais e diagonais.

>Ajude um rato a encontrar um pedaço de queijo num labirinto como o do desenho da figura 1: Um labirinto desses pode ser representado por uma matriz retangular L, cujo elemento $L[i][j]$ vale 0 ou −1 conforme a casa correspondente do labirinto seja uma passagem livre ou uma parede, respectivamente.

<p align="center">
  <img src ='https://raw.githubusercontent.com/rafaeldjsm/Matematica/master/imagens/rato_labirinto2.PNG' width=500px></p>
 

|    |   0 |   1 |   2 |   3 |   4 |   5 |   6 |   7 |   8 |   9 |   10 |
|---:|----:|----:|----:|----:|----:|----:|----:|----:|----:|----:|-----:|
|  0 |  12 |  11 |  -1 |  -1 |   8 |   7 |   6 |   0 |   0 |   0 |    0 |
|  1 |   0 |  -1 |  10 |   9 |  -1 |   0 |  -1 |   5 |  -1 |  -1 |    0 |
|  2 |   0 |   0 |  -1 |   0 |  -1 |   0 |  -1 |   0 |   4 |   0 |   -1 |
|  3 |   0 |  -1 |   0 |  -1 |   0 |   0 |   0 |  -1 |  -1 |   3 |    0 |
|  4 |   0 |   0 |   0 |  -1 |   0 |  -1 |   0 |   0 |   0 |  -1 |    2 |
|  5 |   0 |  -1 |   0 |   0 |   0 |   0 |   0 |   0 |  -1 |   0 |    1 |

<table border="1" class="dataframe" align: center>
  <thead>
    <tr style="text-align: center;">
      <th></th>
      <th>0</th>
      <th>1</th>
      <th>2</th>
      <th>3</th>
      <th>4</th>
      <th>5</th>
      <th>6</th>
      <th>7</th>
      <th>8</th>
      <th>9</th>
      <th>10</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>12</td>
      <td>11</td>
      <td>-1</td>
      <td>-1</td>
      <td>8</td>
      <td>7</td>
      <td>6</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
    </tr>
    <tr>
      <th>1</th>
      <td>0</td>
      <td>-1</td>
      <td>10</td>
      <td>9</td>
      <td>-1</td>
      <td>0</td>
      <td>-1</td>
      <td>5</td>
      <td>-1</td>
      <td>-1</td>
      <td>0</td>
    </tr>
    <tr>
      <th>2</th>
      <td>0</td>
      <td>0</td>
      <td>-1</td>
      <td>0</td>
      <td>-1</td>
      <td>0</td>
      <td>-1</td>
      <td>0</td>
      <td>4</td>
      <td>0</td>
      <td>-1</td>
    </tr>
    <tr>
      <th>3</th>
      <td>0</td>
      <td>-1</td>
      <td>0</td>
      <td>-1</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>-1</td>
      <td>-1</td>
      <td>3</td>
      <td>0</td>
    </tr>
    <tr>
      <th>4</th>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>-1</td>
      <td>0</td>
      <td>-1</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>-1</td>
      <td>2</td>
    </tr>
    <tr>
      <th>5</th>
      <td>0</td>
      <td>-1</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>-1</td>
      <td>0</td>
      <td>1</td>
    </tr>
  </tbody>
</table>

Figura 2 - Matriz

### Saída de Dados 

>A saída do seu programa deve ser uma lista de coordenadas que comece pela posição inicial do rato e termine na posição inicial do queijo. Essa sequencia de coordenadas deve indicar o caminho mais curto para o rato chegar ao queijo.
