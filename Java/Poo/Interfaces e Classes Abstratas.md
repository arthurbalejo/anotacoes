[[Poo]]

Interface - modelo que define um contrato que as classes devem seguir, nao podem ser instanciadas.
Carro é a interface e Sandero/Mobi são classes que implementam essa interface


```
package Java_curso;  
  
public class Main {  
    public static void main(String[] args){  
  
        Carro meuCarro = new Sandero();  
        Carro meuCarro2 = new Mobi();  
  
        meuCarro.acelerar();  
        meuCarro2.acelerar();  
  
    }  
}
```

![[Pasted image 20250123110640.png]]

Classes abstratas - posso colocar metodos sem implementação, assim como na interface, mas, aqui podemos colocar metodos com implementação. Também, nao pode instanciar.

Main.java
```
package Java_curso;  
  
public class Main {  
    public static void main(String[] args){  
  
        Carro meuCarro = new Sandero();  
        Carro meuCarro2 = new Mobi();  
  
        SerVivo meuSer = new Humano();  
        meuSer.respirar();  
  
        meuCarro.acelerar();  
        meuCarro2.acelerar();  
  
    }  
}
```

SerVivo.java
```
package Java_curso;  
  
public abstract class SerVivo {  
  
    protected int idade;  
  
    public SerVivo(int idade){  
        this.idade = idade;  
    }  
  
    public abstract void respirar();  
  
    public void dormir(){  
        System.out.println("Dormindo...");  
    }  
}
```

Humano.java
```
package Java_curso;  
  
public class Humano extends SerVivo{  
  
    public Humano(){  
        super(42);  
    }  
  
    @Override  
    public void respirar() {  
        System.out.println(this.idade);  
        System.out.println("Inalando e exalando CO2 e Oxigenio");  
    }  
}
```

