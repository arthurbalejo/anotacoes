[[Java]]

```
// ArrayList permite a criação de uma lista dinamica  
ArrayList<String> nomes = new ArrayList<>();  
nomes.add("gremio");  
nomes.add("imortal");  
nomes.add("tricolor");  
nomes.add("campeao");  
  
System.out.println(nomes.get(2));  
// vai printar tricolor  
  
nomes.remove(2);  
System.out.println(nomes.get(2));  
// vai printar campeao  
  
nomes.remove("imortal");  
System.out.println(nomes.get(1));  
// vai printar campeao
```
