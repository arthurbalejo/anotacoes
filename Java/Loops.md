[[Java]]

```
// ArrayList permite a criação de uma lista dinamica  
ArrayList<String> nomes = new ArrayList<>();  
nomes.add("gremio");  
nomes.add("imortal");  
nomes.add("tricolor");  
nomes.add("campeao");  
  
for (int i = 0; i < nomes.size(); i++){  
    System.out.println(nomes.get(i));  
}  
  
for (String nome : nomes){  
    System.out.println(nome);  
}  
  
int contador = 0;  
while (contador < 10){  
    System.out.println("estou no while");  
    contador++;  
}
```
