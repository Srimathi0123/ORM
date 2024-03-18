# Ex02 Django ORM Web Application
## Date: 28/02/2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![image](https://github.com/Srimathi0123/ORM/assets/118673240/ef1b6633-fa20-4662-a486-b1ebd620e9ed)


Include your ER diagram here

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
## Models.py
```

 from django.db import models
 from django.contrib import admin
 class Book_DB(models.Model):
  Booknum=models.IntegerField(primary_key="Booknum");
  title=models.CharField(max_length=15);
  Author=models.CharField(max_length=20);
  Date=models.DateField();
  lang=models.CharField(max_length=10);
  price=models.IntegerField();
 class Book_DBAdmin(admin.ModelAdmin):
Include the screenshot of your admin page.
 Thus the program for creating a database using ORM hass been executed successfully
  list_display=("Booknum","title","Author","Date","lang","price");
```

## Admin.py
```
from django.contrib import admin
 from .models import Book_DB,Book_DBAdmin
 admin.site.register(Book_DB,Book_DBAdmin)
```
## OUTPUT
![image](https://github.com/Srimathi0123/ORM/assets/118673240/883aa4d0-0dd0-4d5e-9934-f248f4d660f8)


Include the screenshot of your admin page.


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
