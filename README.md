# Ex02 Django ORM Web Application
## Date: 8.03.2025

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM



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
```
models.py

from django.db import models
from django.contrib import admin
class Book(models.Model):
     bookid=models.IntegerField(primary_
     key=True);
     bookname=models.CharField(max_length=20);
     author=models.CharField(max_length=50);
     price=models.IntegerField();
     publishdate=models.DateField();
class BookAdmin(admin.ModelAdmin):
     list_display=("bookid","bookname","author","price","publishdate");

admin.py
from django.contrib import admin
from .models import Book ,BookAdmin
admin.site.register(Book,BookAdmin)
```

## OUTPUT
![Screenshot 2025-04-26 102358](https://github.com/user-attachments/assets/530e2a44-fae2-4e48-8fda-df16aa0d3c71)



## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
