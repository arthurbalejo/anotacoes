[[Banco de Dados]]

### seleciona a base de dados
```use base_de_dados;```
### mostra as tabelas
```show tables;```
### descreve as colunas das tabelas
```describe users;```
### inserir registros
```INSERT into users (first_name, last_name, email, password_hash) VALUES ("Helena", "A.", "1@email.com", "3_hash"), ("Joana", "B.", "2@email.com", "4_hash"), ("Rosana", "C.", "3@email.com", "5_hash");```
### seleciona colunas * = all
```SELECT * from users as u;```
### selecionando algumas colunas
```SELECT email, id from users as u;```
### selecionando sem dar problema em join com colunas de mesmo nome
```SELECT u.email, u.id, u.first_name from users as u;```
### where filtra registros int
```SELECT * from users where id=3;```
### where filtra registros string
```SELECT * from users where first_name ="Helena";```
### where filtra registros com operadores = < > <= >= !=
```SELECT * from users where id>3;```
### where filtra com condicoes and or
```SELECT * from users where id>3 and last_name = "B.";```
### where filtra com condicoes and or
```SELECT * FROM users where created_at <= '2021-12-03 20:48:09' AND created_at >= '2021-09-04 11:33:50';```
### between seleciona um range
```SELECT * FROM users where created_at BETWEEN '2021-08-28 19:44:45' AND '2021-12-03 20:48:09' and id BETWEEN 18 and 50;```
### in seleciona elementos entre os valores enviados (filtra valores dentro de um alista de valores)
```SELECT * from users WHERE id in (80, 85, 90);```
### like filtra valores que contem determinado valor valor parecido/ % significa qualquer coisa antes do a
```SELECT * from users where first_name like '%mo%';```
### usando like para filtrar por numero de caracteres
```SELECT * from users where first_name like '___';```
### ORDER BY, da pra ordenar por mais de uma coluna sendo que a primeira eh a principal
```SELECT id, first_name, email from users WHERE id BETWEEN 100 AND 150 ORDER BY created_at asc;```
### LIMIT limita quantidade de valores
```SELECT id, first_name, email from users WHERE id BETWEEN 100 AND 150 ORDER BY first_name DESC LIMIT 3;```
### offset a partir do...
```SELECT id, first_name, email from users WHERE id BETWEEN 100 AND 150 ORDER BY id asc LIMIT 2 OFFSET 4;```