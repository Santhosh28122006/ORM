# Ex02 Django ORM Web Application
# Date:18.10.2024
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

# PROGRAM
'''
admin.py

from django.contrib import admin
from .models import book,bookadmin

admin.site.register(book,bookadmin)

models.py

from django.db import models
from django.contrib import admin

class book(models.Model):
    book_name=models.CharField(max_length=100)
    book_price=models.IntegerField()
    author=models.CharField(max_length=100)
    genre=models.CharField(max_length=100)
    language=models.CharField(max_length=100)

class bookadmin(admin.ModelAdmin):
    list_display=('book_name','book_price','author','genre','language')



'''
# OUTPUT
![Screenshot 2024-12-06 223631](https://github.com/user-attachments/assets/8a49de84-a914-4ca3-b3fd-239e3acf44b4)
![Screenshot 2024-12-06 225524](https://github.com/user-attachments/assets/5a711226-314b-48d3-b1f2-2ddfe0c3236e)



# RESULT
Thus the program for creating a database using ORM hass been executed successfully
