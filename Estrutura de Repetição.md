#### Estrutura de Repetição

* O real poder dos computadores está na sua habilidade para repetir uma operação ou uma série de operações várias vezes.
* Cada repetição é chamada laço (loop) é um dos conceitos básicos da programação estruturada.
* Uma estrutura de repetição permite que uma sequência de comandos seja executada repetidamente, caso determinadas condições sejam satisfeitas.
* Essas condições são representadas por expressões lógica.
* As estruturas de repetição podem ser classificadas em:
  * Repetição com teste no início (while)
  * Repetição com teste no final (do-while)

* O comando `break` é utilizado para terminar de forma abrupta uma repetição.
*  O comando `continue` quando é executado, os comandos restantes da repetição são ignorados e programa volta a testar novamente ou não.

___

#### Operadores de Incremento e Decremento

##### PRÉ-FIXADOS:

| Para                                      | Use o atalho | Foma original                                   |
| ----------------------------------------- | ------------ | ----------------------------------------------- |
| Somar uma unidade ao valor da variável    | `++numero`   | `numero = numero + 1;         (retorne numero)` |
| Subtrair uma unidade do valor da variável | `--numero`   | `numero = numero - 1;         (retorne numero)` |

##### PÓS-FIXADOS:

| Para                                                         | Use o atalho | Foma original                              |
| ------------------------------------------------------------ | ------------ | ------------------------------------------ |
| Somar uma unidade ao valor da variável, retornando o valor original. | `numero++`   | `(retorne numero)    numero = numero + 1;` |
| Subtrair uma unidade do valor da variável, retornando ao valor original. | `numero--`   | `(retorne numero)    numero = numero - 1;` |

##### Operações Aritméticas:

| Para:                                        | Use o atalho:  | Forma original:        |
| -------------------------------------------- | -------------- | ---------------------- |
| Somar `i`  unidades ao  valor da variável    | `numero += i;` | ` numero = numero + i` |
| Subtrair `i`  unidades ao  valor da vraiável | `numero -= i;` | `numero = numero - i`  |
| Multiplicar o valor da variável por `k`      | `numero *= k;` | `numero = numero * k;` |
| Dividir o valor da variável por `k`          | `numero /= k;` | `numero = numero / k;` |

___

#### Arrays

* Array é um objeto utilizada para armazenar sequencialmente dados do mesmo tipo.

* Permanecem com o mesmo tamanho depois de criado.

  * ##### Array Unidimensional:

    | Nome do Array c[n] | Dados do array |
    | ------------------ | -------------- |
    | c[0]               | -45            |
    | c[1]               | 6              |
    | c[2]               | 0              |
    | c[3]               | 72             |
    | c[4]               | 1543           |
    | c[5]               | -89            |
    | c[6]               | 0              |
    | c[7]               | 62             |
    | c[8]               | -3             |
    | c[9]               | 1              |
    | c[10]              | 6453           |
    | c[11]              | 1942           |
    | c[12]              | 33             |

  

  

  * ##### Array Multimensional:

    | array = a[i] [j] | `Coluna 0` | `Coluna 1` | `Coluna 2` | `Coluna 3` |
    | ---------------- | ---------- | ---------- | ---------- | ---------- |
    | **`Linha`0**     | `a[0] [0]` | `a[0] [1]` | `a[0] [2]` | `a[0] [3]` |
    | **`Linha 1`**    | `a[1] [0]` | `a[1] [1]` | `a[1] [2]` | `a[1] [3]` |
    | **`Linha 2`**    | `a[2] [0]` | `a[2] [1]` | `a[2] [2]` | `a[2] [3]` |

    