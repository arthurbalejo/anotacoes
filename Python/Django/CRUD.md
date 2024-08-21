Criando objetos

```
# Course instance
course_cloud_app =  Course(name="Cloud Application Development with     Database", description = "Develop and deplot application on cloud")

course_cloud_app.save()

# Project instance
project_orm = Project(name="Object-relational mapping project", grade=0.2, course = course_cloud_app) # course_cloud_app -> foreingkey

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
