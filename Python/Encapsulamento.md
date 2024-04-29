[[Python]]
Uma das principais vantagens do conceito de orientação a objetos é a **utilização de estruturas sem a necessidade de conhecer como elas foram implementadas**.

Para isso, o conceito de **encapsulamento de dados torna-se essencial**, pois envolve a **proteção dos atributos ou métodos de uma classe**.

A ideia de encapsular o código vem com a premissa de proteger atributos e métodos de uma classe (tornando-os privados), de forma que somente a classe onde as declarações foram feitas tenham acesso.

Esse conceito garante a integridade das informações e também facilita a utilização das implementações.

De forma geral, todas as linguagens de programação que utilizam orientação a objetos usam modificadores de acesso para alterar a visibilidade de classes, atributos e métodos.

Para a implementação do encapsulamento é fundamental alterarmos a visibilidade dos atributos de uma classe. Para isso, utilizamos os modificadores de acesso.

Diferentemente de outras linguagens, como o Java e o C#, que utilizam palavras reservadas, a linguagem Python utiliza o símbolo underscore ”_”.

Dentro da orientação a objetos temos os modificadores Public, Protected e Private.

Public: É o mais comum entre os modificadores.
Ele permite acesso tanto de dentro, quanto de fora de uma classe.
Sua implementação se dá por meio do uso do underline ” _ ” na frente do nome.

Protected: Utilizando o modificador protegido, somente suas classes e subclasses terão acesso ao atributo ou método.
Para sua implementação adicione um underline ” _ ” antes do nome.

Private: É o modificador mais restrito do desenvolvimento orientado a objetos.
Ele permite que somente a sua classe (onde foi definido) tenha acesso a um determinado atributo ou método.
Para definir o método private adicionamos underline duplo ” __ ” na frente do nome.

Get
Sempre retornam valores.
O método Get é utilizado para ler os valores internos do objeto e enviá-los como valor de retorno da função.

get_nome do atributo()
Exemplo:
get_idade(self):return self._idade

Set
Recebem valores por parâmetros.
Os métodos Set recebem argumentos que serão atribuídos a membros internos do objeto.

set_nome do atributo
(valor por parâmetro)
Exemplo:
def set_idade(self, valor):
self.idade=valor

Decorados:
Um decorator é um padrão de projeto de software que permite adicionar comportamento a um objeto já existente, em tempo de execução, ou seja, agrega, de forma dinâmica, responsabilidades adicionais a um objeto.
Na prática, o decorator permite que atributos de uma classe tenham responsabilidades.
Um decorator é um objeto invocável, uma função que aceita outra função como parâmetro (a função decorada).
O decorator pode realizar algum processamento com a função decorada e devolvê-la ou substituí-la por outra função.

@Property:
A linguagem Python traz uma outra solução para manter os atributos privados, conhecida como Property.
A função Property é um Decorator e é utilizada para obter um valor de um atributo.
Basicamente, a função Property permite que você declare uma função para obter o valor de um atributo.