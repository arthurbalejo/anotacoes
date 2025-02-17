[[Poo]]

Classes -  modelo que define a estrutura dos objetos. os atributos e métodos que o objeto possui.

Atributos - variaveis de uma classe

Metodos - funções que uma classe possui

```
public class Main {  
    public static void main(String[] args){  
  
        Carro meuCarro = new Carro("Fusca");  
        Carro meuCarro1 = new Carro("Sandero");  
        Carro meuCarro2 = new Carro("BMW");  
  
        meuCarro.acelerar();  
        meuCarro1.acelerar();  
        meuCarro2.acelerar();  
  
    }  
}  
  
class Carro{  
    //atributos  
    String modelo;  
  
    //construtor  
    public Carro(String modelo){  
        this.modelo = modelo;  
    }  
      
    //metodo  
    public void acelerar(){  
        System.out.println("Acelerando o carro " + this.modelo);  
    }  
}
```




