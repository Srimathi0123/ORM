# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

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
## models.py

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


Include your code here

## OUTPUT
![image](https://github.com/selvasachein/ORM/assets/118673240/2af69dc5-a77e-47fd-a397-b1aec68cf245)

Include the screenshot of your admin page.


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
