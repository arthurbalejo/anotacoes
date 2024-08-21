[[Python]]

Transformando csv em data frame

```
import pandas as pd

csv_path = "file1.csv"

df = pd.read_csv(csv_path)
```

Ver a primeira linhas

```
df.head()
```

iloc para acessar celulas individuais -> acessando primeiro conteudo da primeira coluna
```
df.iloc[0,0]
```
da para utilizar o nome da coluna também -> acessando primeiro conteudo da coluna artist
```
df.iloc[0,'artist']
```

Recortando um dataframe -> linhas de 0 até 2 e colunas 0 até 3

```
z = df.iloc[0:2, 0:3]
```

usando loc

```
z = df.loc[0:2, 'artist':'Released']
```

Elementos unicos de uma coluna

```
df['Released'].unique()
```

Usando operadores -> filtrando, o resultado é uma coluna com valores booleanos

```
df['Released'] > 1979
```

Exportando um dataframe

```
df1.to_csv('new_songs.csv')
```

