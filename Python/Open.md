[[Python]]

## READING

file object = open( "path" , "r" ) r para reading

```
file1 = open("/resources/data/Example1.txt","r")
file1.close()
```

se usar o with ele fecha o metodo open automaticamente

```
with open("Example.txt", "r") as file1
	file_stuff = file1.read()
```

com o readline() cada linha vira um elemento dentro de uma lista

```
with open("Example.txt", "r") as file1
	file_stuff = file1.readline()
	
print(file_stuff[2])
```

eu posso ler até determinando elemento com o read(elemento)

```
with open("Example.txt", "r") as file1
	file_stuff = file1.read(16)
	
print(file_stuff[2])
```

## WRITING

vai criar um arquivo Example2.txt no meu diretorio

```
with open("/resources/data/Example2.txt", "w") as file1
	file.write("This is line A\n")
	file.write("This is line B\n")
```

para escrever varios elementos de uma lista em um arquivo

```
Lines = ["This is line A\n", "This is line B\n", "This is line C\n"]

with open("/resources/data/Example2.txt", "w") as file1
	for line in Lines:
		file.write(line)
```

para adicionar um elemento ao arquivo e nao reescrever

```
with open("/resources/data/Example2.txt", "a") as file1
	file.write("This is line D")
```

para ler um arquivo e escrever outro com base no primeiro

```
with open("/resources/data/Example1.txt", "r") as readfile
	with open("/resources/data/Example3.txt", "w") as writefile
		for line in readline:
			writefile.write(line)
```
