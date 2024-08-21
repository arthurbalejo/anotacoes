 ![[Pasted image 20240821090012.png]]

```
User and Instructor Django Models

class Instructor(models.Model):
	is_full_time = models.BooleanField()
	total_learners = models.IntergerField()
	user = models.OneToOneField(User) #

class User(models.Model):
	first_name = models.CharField(max_length=30)
	last_name = models.CharField(max_length=30)
	dob = models.CharField(max_length=30)
```

![[Pasted image 20240821090435.png]]

```
Project and Course Django Models

class Project(models.Model):
	name = models.CharField(max_length=30)
	grade = models.CharField(max_length=30)
	course = models.ForeingKey(Course) #

class Course(models.Model):
	name = models.CharField(max_length=30)
	description = models.CharField(max_length=30)

```
![[Pasted image 20240821090931.png]]

```
Project and Learner Django Models

class Course(models.Model):
	name = models.CharField(max_length=30)
	description = models.CharField(max_length=30)
	learners = models.ManyToManiField(Learner)

class Leaner(models.Model):
	occupation = models.CharField(max_length=30)
	social_link = models.URSLField()
```

![[Pasted image 20240821091729.png]]

```
Project and Learner Django Models

class Course(models.Model):
	name = models.CharField(max_length=30)
	description = models.CharField(max_length=30)
	learners = models.ManyToManiField(Instructor, through='Enrollment')

class Enrollment(models.Model):
	course = models.ForeingKey(...)
	learner = models.ForeingKey(...)
	date_enrroled = models.DateField()
	
class Leaner(models.Model):
	occupation = models.CharField(max_length=30)
	social_link = models.URSLField()
```

![[Pasted image 20240821092439.png]]

![[Pasted image 20240821092456.png]]![[Pasted image 20240821092606.png]]


