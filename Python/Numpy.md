[[Python]]

Transformando uma lista em numpy array

```
import numpy as np

a = np.array([0,1,2,3,4])
```

```
a.size #tamanho array -> 5

a.ndim #dimensões do array -> 1

a.shape #tupla com quantas linhas e colunas -> (5,1)
```

Alterando valores de um np array

```
C = np.array([20,1,2,3,4])

C[0] = 100 # C -> [100,1,2,3,4]
```

Recortando np array

```
C = np.array([100,1,2,3,4])

C[3:5] = 300,400 #C -> [100,1,2,300,400]
```

Somando vetores

```
u = np.array([1,0])
v = np.array([0,1])

z = u + v #Z -> [1,1]
```

Produto de vetores

```
y = np.array([1,2])

z = 2*y #Z -> [2,4]
```
com dois arrays
```
u = np.array([1,2])
v = np.array([3,2])

z = u*v #z -> [3,4]

#usando dot para produto escalar
result = np.dot(u,v) #result -> 5 (1*3 + 2*1)
```

Adicionando uma constante

```
u = np.array([1,2,3,-1])

z = u+1 3 #Z -> [2,3,4,0]
```

Funções universais

```
a = np.array([1,-1,1-1])

mean_a = a.mean()

max_a = a.max()
```

Aplicando uma função em cada elemento do np array

```
x = np.array([0, np.pi/2, np.pi]) #[0,pi/2,pi]

y = np.sin(x) # y -> [sin(0),sin(pi/2),sin(pi)]
```

Gerando numeros

```
np.linspace(-2,2,num=9)

#-2 até 2 é o intervalo e 9 a quantidade de numeros gerados
```

Plotando funções

```
x = np.linspace(0,2*np.pi,100)
y = np.sin

import matplotlib.pyplot as plt

plt.plot(x,y)
```

Duas dimensões

```
a = [[11,12,13],[21,22,23],[31,32,33]]

A = np.array(a)

A.ndim # 2

A.shape # (3,3)

A.size # 3*3 = 9
```