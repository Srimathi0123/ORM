# Ex02 Django ORM Web Application
## Date:28.02.2024 

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![image](https://github.com/selvasachein/ORM/assets/118673240/4243876c-c802-45f7-9ec3-8eff10453a1e)

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
  list_display=("Booknum","title","Author","Date","lang","price");
```
## admin.py
```
from django.contrib import admin
from .models import Book_DB,Book_DBAdmin
admin.site.register(Book_DB,Book_DBAdmin)
```

## OUTPUT
![image](https://github.com/selvasachein/ORM/assets/118673240/30af3eda-c0e1-4d06-8829-cdc8487e0bc8)


Include the screenshot of your admin page.


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
