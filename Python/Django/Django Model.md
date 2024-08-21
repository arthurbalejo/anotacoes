[[Python]]
[[Banco de Dados]]

![[Pasted image 20240821085123.png]]

```
User model
class User(models.Model):
	first_name = models.CharField(max_length=30)
	...
```

DJANGO ORM transforma em
```
Table create statement

CREATE TABLE data_user
(
	"id" serial NOT NULL PRIMARY KEY,
	"first_name" varchar(30) NOT NULL,
	...
)
```

com varios campos
```
User model
class User(models.Model):
	first_name = models.CharField(max_length=30)
	last_name = models.CharField(max_length=30)
	dob = models.DateField()
```

DJANGO ORM transforma em
```
Table create statement

CREATE TABLE data_user
(
	"id" serial NOT NULL PRIMARY KEY,
	"first_name" varchar(30) NOT NULL,
	"last_name" varchar(30) NOT NULL,
	"dob" date NOT NULL
	
),
```
