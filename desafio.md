```java
import java.io.BufferedReader; // classe que permite que permitem a  leitura da entrad no formato que é pedido.
import java.io.InputStreamReader;
import java.io.IOException;
import java.util.StringTokenizer;

public class MinhaPrimeiraClase {
    public static void main(String[] args) thrwos IOException{
        BufferReader br = new BufferedReader(new InputStreamReader(System.in));
        StringTokenizer st = new StringTokenizer(br.readLine());
        int a = Integer.parseInt(st.nextToken());//pimentoes amarelos
        int b = Integer.parseInt(st.nextToken());//pimentoes vermelhos
        int total = a + b; //Altere o valor da variável com o cálculo esperado
        System.out.pritnln("X = " + total);
    }
}
```

