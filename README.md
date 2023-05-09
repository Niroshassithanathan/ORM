# Ex02 Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a student database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![ORM1](https://user-images.githubusercontent.com/121418437/236993176-3f956a6c-2f84-4272-a95b-d471a392edf3.jpg)

## DESIGN STEPS

### STEP 1:

Clone the problem from github

### STEP 2:

Create a new app

### STEP 3:

Enter the code for admin.py and model.py

### STEP 4:

Execute Django admin and create 10 employees

## PROGRAM
```
Models.py 

from django.db import models
from django.contrib import admin
class Student (models.Model):
    regno=models.IntegerField()
    name=models.CharField(max_length=100)
    marks=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()
     
class StudentAdmin(admin.ModelAdmin):
    list_display=('regno','name','marks','age','email')
    
Admin.py 

from django.contrib import admin
from .models import Student,StudentAdmin
admin.site.register(Student,StudentAdmin)
```
## OUTPUT

![ORM2](https://user-images.githubusercontent.com/121418437/236993062-5566d490-ec54-44a1-b9a9-2d2386730cff.jpg)

## RESULT
Program executed successfully.
