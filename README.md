o# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
clone the problem from github
### STEP 2:
create a new app in django project
### STEP 3:
Enter the code for admin.py and models.py
### STEP 4:
Execute django admin and create username.

## PROGRAM
~~~
models.py
from django.db import models
from django.contrib import admin
# Create your models here.
class Student (models.Model):
referencenumber=models.CharField(max_length=20,help_text="reference 
number")
 name=models.CharField(max_length=100)
 age=models.IntegerField()
 email=models.EmailField()
 mobileno=models.IntegerField()
class StudentAdmin(admin.ModelAdmin):
 list_display=
('referencenumber','name','age','email','mobileno')
 admin.py
 from django.contrib import admin
from .models import Student, StudentAdmin
# Register your models here.
admin.site.register(Student,StudentAdmin)
~~~
## OUTPUT

![image](https://github.com/RESHMA22C/django-orm-app/assets/147474426/bf3f977d-b67b-42f7-8805-8c023eef9b53)



## RESULT
The program for creating a database using ORM has been executed sucessfully.
