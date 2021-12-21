#### Conceituação

> São estruturas que possuem a capacidade de direcionar o fluxo de execução do código



#### Tipos:

* Decisão: Estrutura que avalia uma condição booleana ou variável para direcionar o fluxo de execução.

  * Opções: if(se), if-else(se-senão), if-else-if(se-senão-se), switch(escolha) e operador ternário

    ```java
    // if(se)
    if(condição){
    }
    ```

    ```java
    // if-else(se-senão)
    if(condição){
    } else{
    }
    ```

    ```java
    // if-else-if(se-senão-se)
    if(condição){
    }else if(condição){
    }else{
    }
    ```

    ```java
    //operador ternário
    condição ? true : false;
    // ou 
    condição ? true : null;
    ```

    ```java
    // switch
    switch(variável){
        case 1:
            break;
        case 2:
            break;
        default:
            break;
    }
    ```

    

  #### Boas práticas

  * Switch é para valores exatos e if para expressões booleanas

  * Evitar usar o default do switch para "cases genérico"

  * Evitar o efeito "flecha" do if's

  * Evitar muitos if's aninhados

  * Usar a boa prática da aula 2 para diminuir o tamanho do if

    ____

    

* Repetição: `for`

  * Estrtura básica do `for` : 

    `for (início; fim; incremento){`

    ​	`//códigos`

    `}`

    onde: 

    - início: expressão que indica o ponto de início.

    - fim: expressão que indica quando parar.

    - incremento: expressão faz o "`for` caminhar".

      

  * `for` each

    ```java
    for(<TipoDeDado> variável: itens){
    	//códigos
    }
    ```

    

  * `for` com interator:

    ```java
    for(Iterator<TipoDeDado> <nomeVariável> = itens.iterator(); itens.hasNext(); ){
    	//códigos
    }
    ```

    

  * `for` com loop inifinito

    ```java
    for( ; ; ){
    	//códigos
    	}
    
    
    ```

    ____

    

*  `while` onde: 

* expressão: expressão booleana que permite e controla a execução do `while`.

  * Estrutura básica do `while` :

    ```java
    while (expressão){
    	//código
    }
    ```

    

  * `while` infinito:

    ```java
    while (true){
     //códigos
    //ao final pode se verificar se ainda deve continuar executado.
       }
    ```

    

*  `do` `while` :

  * ```java
    do {
    	//faz a pergunta do quis
    	//Atualiza a quantidade de tentativas
    } while (tentativas <= limiteTentativas);
    ```

    ____

    

  #### Conceituação

  ##### Interruptores: São comandos que têm a capacidade de modificar o fluxo de execução de loops e métodos."

*  `break` :

  * Interrompe a execução do `for`, `while` e `switch`.
  * opções de uso: 
    * **não** marcada (*unlabeled*)
    * marcada (*labeled*)

* `continue` :

  * Intrerrompe parciamente a execução do `for`, `while`.
  * opções de uso: 
    * **não** marcada (*unlabeled*)
    * marcada (*labeled*)

* `return`

  * Intorrompe a execução do método.
  * Opções de uso: com valor e sem valor.


____

