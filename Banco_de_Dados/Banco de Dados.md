### SELECT

```
SELECT column1, column2 FROM table_name;
```

### FROM

```
SELECT column1, column2 FROM table_name;
```


### WHERE

```
SELECT column1, column2 FROM table_name WHERE condition;
```


### ORDER BY

```
SELECT column1, column2 FROM table_name ORDER BY column1 ASC;
```


### GROUP BY

```
SELECT column1, COUNT(*) FROM table_name GROUP BY column1;
```


### HAVING

Filtros agrupados dados com base em condições especificadas.

```
SELECT column1, COUNT(*) FROM table_name GROUP BY column1 HAVING COUNT(*) > 1;
```


### INSERT INTO

```
INSERT INTO table_name (column1, column2) VALUES (value1, value2);
```


### UPDATE

```
UPDATE table_name SET column1 = value1 WHERE condition;
```


### DELETE FROM

```
DELETE FROM table_name WHERE condition;
```


### JOIN

Combina linhas de várias tabelas com base em colunas relacionadas.

```
SELECT column1, column2 FROM table1 JOIN table2 ON table1.column = table2.column;
```


### INNER JOIN

Retorna apenas linhas correspondentes de ambas as tabelas.

```
SELECT column1, column2 FROM table1 INNER JOIN table2 ON table1.column = table2.column;
```


### LEFT JOIN

Retorna todas as linhas da tabela esquerda e linhas correspondentes da tabela direita.

```
SELECT column1, column2 FROM table1 LEFT JOIN table2 ON table1.column = table2.column;
```


### RIGHT JOIN

Retorna todas as linhas da tabela da direita e linhas correspondentes da tabela da esquerda.

```
SELECT column1, column2 FROM table1 RIGHT JOIN table2 ON table1.column = table2.column;
```


### FULL JOIN

Retorna todas as linhas de ambas as tabelas, independentemente da correspondência.

```
SELECT column1, column2 FROM table1 FULL JOIN table2 ON table1.column = table2.column;
```


### DISTINCT

```
SELECT DISTINCT column1 FROM table_name;
```


### COUNT

```
SELECT COUNT(*) FROM table_name; or SELECT COUNT(column1) FROM table_name;
```


### SUM

```
SELECT SUM(column1) FROM table_name;
```


### AVG

```
SELECT AVG(column1) FROM table_name;
```


### MAX

```
SELECT MAX(column1) FROM table_name;
```


### MIN

```
SELECT MIN(column1) FROM table_name;
```



