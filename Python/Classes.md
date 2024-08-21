[[Python]]
O desenvolvimento de uma aplicação envolve os mais diferentes tipos de informações, que são modeladas com estruturas que conhecemos como **classes**.

A partir das classes é possível **criar objetos**, ou seja, uma classe é um “molde” para a criação de objetos.

Podemos afirmar que classe é um **Tipo Abstrato de Dados (TAD)**, ou seja, o código que define e implementa um novo tipo de informação.

Classe: Podemos dizer que a classe é o projeto do objeto, contendo o código de programação.

Objeto: É a execução do código de uma classe. Quando executamos o código de uma classe é criado um novo objeto na memória.
Uma nova instância de um objeto é um tipo abstrato de informação de um novo tipo de dado.

Instancia: Podemos dizer que a instância é o objeto sendo executado.
Quando criamos um novo objeto, afirmamos que estamos criando uma instância dele.

Estrutura da Classe:
	pass: quando nenhuma estrutura seá definida no corpo dessa classe

Declaração dos membros
	Atributos (Propriedades): 
	Os atributos armazenam as características de uma classe. Os atributos são as declarações de variáveis da classe.
	Metodos:
	São ações da classe, suas funções. Representam os estados e ações dos objetos quando instanciados.
	Métodos Construtor:  O Método Construtor é definido de forma implícita ou explícita por todas as classes e, como o próprio nome já cita, é utilizado para construir o objeto. Todas as vezes que um objeto estiver sendo criado (instanciado) é por meio do Construtor que ele será inicializado.  Este método é invocado, automaticamente, pela máquina virtual do Python todas as vezes que um objeto é criado.

Objetos: todo objeto criado possui um código de identificação composto por um número inteiro não negativo conhecido como id.

EXEMPLOS:

Conta.py

```
class Conta:  
    def __init__(self, titular, numero, saldo):  
        self.saldo = 0  
        self.numero = numero  
        self.titular = titular
```

Cliente.py

```
class Cliente:  
    def __init__(self, n, fone):  
        self.nome = n  
        self.telefone = fone

```

Main.py

```
class Main:  
    pass  
  
from Cliente import Cliente  
  
from Conta import Conta  
  
c1 = Cliente("Joao", "114444-2222")  
conta = Conta(c1.nome, 6565, 0)  
  
print(conta.titular, " Numero: ", conta.numero, " Seu Saldo: ", conta.saldo)

```