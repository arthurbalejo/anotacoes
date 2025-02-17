 [[Java]]
inteiros
byte => 8 bits => -128 a 127  
short => 16 bits => -32768 a 32767  
int => 32 bits => -2.147.483.648 a  2.147.483.647  
long => 64 bits => -9.223.372.036.854.775.808 a 9.223.372.036.854.775.807

decimais
float => 32 bits => precisao simples
double => 64 bits => precisao dupla

letras
String => representar palavras e frases
char => representar um unico caractere => a, b, c

boolenos
boolean => true ou false
```
//tipos primitivos
byte b = 100;
short s = 10000;
int i = 1000000;
long l = 1000000L;
float f = 10.5f;
double d = 20.5;
char c = 'A';
boolean bol = true;

//String é uma classe 
String str = "Gremio";
```

Funções String

- Formatar: toLowercase(), toUpperCase(), trim()
- Recortar: substring(inicio), substring(inicio, fim)
- Substituir: Replace(char, char), Replace(String, String)
- Buscar: IndexOf, LastIndexOf
- str.Split(" ")
```
package Java_curso;  
  
public class Main {  
    public static void main(String[] args){  
  
        String original = "abcde FGHIJ ABC abc DEFG    ";  
  
        String s01 = original.toLowerCase();  
        String s02 = original.toUpperCase();  
        String s03 = original.trim();  
        String s04 = original.substring(2);  
        String s05 = original.substring(2, 9);  
        String s06 = original.replace('a', 'x');  
        String s07 = original.replace("abc", "xy");  
        int i = original.indexOf("bc");  
        int j = original.lastIndexOf("bc");  
  
        System.out.println("-" +original + "-");  
        System.out.println("-" + s01 + "-");  
        System.out.println("-" + s02 + "-");  
        System.out.println("-" + s03 + "-");  
        System.out.println("-" + s04 + "-");  
        System.out.println("-" + s05 + "-");  
        System.out.println("-" + s06 + "-");  
        System.out.println("-" + s07 + "-");  
        System.out.println("Index of 'bc': " + i);  
        System.out.println("Last index of 'bc': " + j);  
  
    }  
}
```

Saida:
```
-abcde FGHIJ ABC abc DEFG    -
-abcde fghij abc abc defg    -
-ABCDE FGHIJ ABC ABC DEFG    -
-abcde FGHIJ ABC abc DEFG-
-cde FGHIJ ABC abc DEFG    -
-cde FGH-
-xbcde FGHIJ ABC xbc DEFG    -
-xyde FGHIJ ABC xy DEFG    -
Index of 'bc': 1
Last index of 'bc': 17

Process finished with exit code 0
```

Split:
```
String original = "abcde FGHIJ ABC abc DEFG    ";
String [] vect = original.split(" ");  
System.out.println(vect[0]);  
System.out.println(vect[1]);  
System.out.println(vect[2]);
```

Saida:
```
abcde
FGHIJ
ABC

Process finished with exit code 0
```
