Instalando a JVM

`sudo apt install curl`

* Instalando Java Version Manager:
  * https://github.com/shyiko/jabba
  * `curl -sl https://github.com/shyiko/jabba/raw/master/install.sh | bash && . ~/.jabba/jbba.sh`

```
ozeias@barreto:~$ export JABBA_VERSION=0.11.2
ozeias@barreto:~$ curl -sL https://github.com/shyiko/jabba/raw/master/install.sh | bash && . ~/.jabba/jabba.sh
Installing v0.11.2...

Adding source string to /home/ozeias/.bashrc
Adding source string to /home/ozeias/.bash_profile

Installation completed
(if you have any problems please report them at https://github.com/shyiko/jabba/issues)
ozeias@barreto:~$ 

```

` jabba ls-remote` :  lista todas as versões disponiveis

Para instalar: 

`jabba install ...versão...`

`jabba ls` : para listar as versões instaladas no SO

`jabba use ...versão...`: para usar a versão que se quer.

`java -version`: para verificar a versão que está em uso:

#### Executando um programa JAVA

* Criando classe principal(src/com/dio/MyFirstProgram.java) :

```java
package com.dio;
import com.dio.base.Oder;

public class MyFirsrtProgram {
	public static void main (String[] args){
	final Order order= new Order("code1234");
	System.out.println(order)
	}
}
```

* Criando classe Order e seus metodos (src/com/dio/Order.java) :

```java
package com.dio.base;

public class Order{
	private final String code;
	
	public Order(String code){
		this.code = code;
	}
	@Override
	public String toString(){
		return "Order={" + 
        		"code='" + code + "'"
        		"}";
	}
}
```

* Copilando:

  ```
  jabba use openjdk@1.11
  javac -d target/ -sourcepath src/ src/com/dio/MyFirstProgram.java
  ```

  

* Executar:

  ```
  cd target/
  java com.dio.MyFirstProgram
  ```

  