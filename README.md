# Ex02 Django ORM Web Application
## Date: 23.04.2025

## AIM
To develop a Django application to store and retrieve data from Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

![orm diagram](https://github.com/user-attachments/assets/1396d90c-c0bd-4a78-919f-fbf0ac1f05d3)


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
admin.py
from django.db import models
from django.contrib import admin

models.py
class Movie(models.Model):
    user_id = models.CharField(max_length=20, help_text="User ID")
    user_name = models.CharField(max_length=100)
    email_id = models.EmailField()
    phone_number = models.CharField(max_length=15)
    movie_name = models.CharField(max_length=200)
    show_datetime = models.DateTimeField()
    no_of_seats = models.IntegerField()

class MovieAdmin(admin.ModelAdmin):
    list_display = ('user_id', 'user_name', 'email_id', 'phone_number', 'movie_name', 'show_datetime', 'no_of_seats')
```


## OUTPUT :
![output orm](https://github.com/user-attachments/assets/45836282-5390-4b5e-9e83-eb560db148a1)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
