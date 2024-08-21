Criando objetos

```
# Course instance
course_cloud_app =  Course(name="Cloud Application Development with
                           Database",
                           description = "Develop and deplot application on                            cloud")

course_cloud_app.save()

# Project instance
project_orm = Project(name="Object-relational mapping project", grade=0.2, 
                      course = course_cloud_app) 
                      #course_cloud_app -> foreingkey
project_orm.save()
```

### Select

SQL - SELECT * FROM Course
```
courses = Course.object.all()

#courses -> QuerySet 
#Course -> Model que eu defini ao criar
#object -> gerenciador modelo padrao, database interface
#all() -> metodo para copiar os resultados da query
```

Filtro
```
part_time_instructors = Instructor.objects.flter(is_full_time=False)
```

exclusao
```
filtered_instructors = Instrictor.objects.exclude(full_time=False).
                                  filter(total_learners__gt=30000).
                                  filter(first_name___startwith='J')
```

para pegar um unico objeto
```
instructor_john = Intstructor.objects.get(first_name='John')
print(instructor_john)
```
output
```
First name: John,
Last name: Doe,
Is full time: True,
Total Learners: 30050
```

![[Pasted image 20240821105555.png]]

### UPDATE

```
learner_john.dob = date(1985, 3, 16)
learner_john.save()
```

com foreingkey

```
project_orm.course = course_python
project_orm.save()
```

com ManyToMany

```
course_python.learners.add(learner_joe)
course_python.save()
```

### DELETE

```
project_orm.delete()
```

deletar todos os cursos cujo nome contem Python

```
Course.objects.filter(name__contains='Python').delete()
```

