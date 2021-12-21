#### O que são operadores lógicos ?

> São símbolos especiais quais são capazes de realizar comparações lógicas entre operandos lógicos ou expressões e, em seguida, retornar um resultado.

#### Tipos:

* Conjunção
* Disjunção
* Disjunção exclusiva
* Negação

____

#### Conceituação

Tipos:

* Conjunção: operação lógica que só é verdadeira quando ambos os operandos ou expressões envolvidas são verdade.

Simbologia:									

* &&

Terminologia:

* and(e)

| O - E | O - E |  R   |
| :---: | :---: | :--: |
|   V   |   V   |  V   |
|   V   |   F   |  F   |
|   F   |   V   |  F   |
|   F   |   F   |  F   |

O - Operando; E - Expressão; R - Resultado

____

* Disjunção: operação que só é falsa quando ambos os operandos ou expressões envolvidos são falsos.

Simbologia:									

* ||

Terminologia:

* or(ou)

| O - E | O - E |  R   |
| :---: | :---: | :--: |
|   V   |   V   |  V   |
|   V   |   F   |  V   |
|   F   |   V   |  V   |
|   F   |   F   |  F   |

O - Operando; E - Expressão; R - Resultado

____

* Disjunção exclusiva: operação que só é verdade quando ambos os operandos ou expressões são opostos

Simbologia:									

* ^

Terminologia:

* xor

| O - E | O - E |  R   |
| :---: | :---: | :--: |
|   V   |   V   |  F   |
|   V   |   F   |  V   |
|   F   |   V   |  V   |
|   F   |   F   |  F   |

O - Operando; E - Expressão; R - Resultado

____

* Negação: operação que inverte o valor lógico de um operando ou expressão

Simbologia:									

* !

Terminologia:

* inversão

| O - E |  R   |
| :---: | :--: |
|   V   |  F   |
|   F   |  V   |

O - Operando; E - Expressão; R - Resultado

____

#### Curiosidade

* Operadores biwise: & e |
* Operadores shift: ~, >>, >>>, <<

____

#### Exemplos

boolean b1 = true; boolean b2 = false;

boolean b3 = true; boolean b4 = false;



b1 && b2, b1 && b3

b2 || b3, b2 || b4

b1 ^ b3, b4 ^ b1

!b1, b2

(i1 > i2) || (f2 < f1)

((i1 + i2) < (f2 - f1)) && true

____

#### Boas práticas

* Crie variáveis auxiliares para guardar resultados intermediários.

`(salarioMensal < mediaSalario) && (quantidadeDependentes >= mediaDependentes)`

​		pode ser

`(salarioBaixo) && (muitosDependentes)`

`boolean recebeAuxilio = (salarioBaixo) && (muitosDependentes);`