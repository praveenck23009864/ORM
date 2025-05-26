# Ex02 Django ORM Web Application
## Date: 18-05-2025

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM
![image](https://github.com/user-attachments/assets/f59abaac-798a-4dcb-972a-9ffd7e456215)


## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM
~~~
admin.py

from django.contrib import admin 
from .models import Employee, EmployeeAdmin 
admin.site.register (Employee, EmployeeAdmin)

models.py

from django.db import models 
from django.contrib import admin
class Employee (models.Model):
    eid=models.CharField(max_length=20,help_text="Employee ID")         
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models. EmailField()

class EmployeeAdmin (admin. ModelAdmin):
    list_display=('eid', 'name', 'salary', 'age', 'email')
~~~


## OUTPUT
![393369624-94b98a73-c2b6-4c8b-949d-87021d5ec283](https://github.com/user-attachments/assets/e786d61c-46a5-4123-8d91-8db280f6b072)
![395064284-941d5f2e-2a21-4f39-8da1-d2e834886a51](https://github.com/user-attachments/assets/140efdfb-d6a7-4074-a80b-32a95726998e)
![393369647-7943d4a5-772d-46c4-ad9d-3cefc1f8f1d1](https://github.com/user-attachments/assets/0f94a8bc-3daf-4f40-ae28-1bafc064328c)
![393369685-3a8a3b5c-2dc6-4ddc-bf9d-7db243feb7b5](https://github.com/user-attachments/assets/ec493fe7-6d84-4a62-a287-25b3343bb52d)




## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
