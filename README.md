# Ex02 Django ORM Web Application
# Date:19-3-2025
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM

![ORM DR](https://github.com/user-attachments/assets/6c9d7cdd-b0e7-4b1e-aada-8872c8c98686)

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
1.models.py
```

from django.db import models
from django.contrib import admin

class Book(models.Model):
  Name= models.CharField(max_length=100)
  Email= models.EmailField()
  Book_No= models.CharField(max_length=100)
  Book_Name= models.CharField(max_length=100)
  Address= models.CharField(max_length=255)
  Phone_No= models.CharField(max_length=15)
class BookAdmin(admin.ModelAdmin):
    list_display = ('Name','Email','Book_No','Book_Name','Address','Phone_No')
```
2.admin.py
```
from django.contrib import admin
from .models import Book, BookAdmin
admin.site.register(Book, BookAdmin)
```
# OUTPUT
Include the screenshot of your admin page.
![Screenshot 2025-03-21 222831](https://github.com/user-attachments/assets/54967d66-5b96-44f6-9939-73329aa80f98)
![Screenshot 2025-03-21 222925](https://github.com/user-attachments/assets/4fd516ed-0291-47cd-b85e-27b3ccd92d72)
![Screenshot 2025-03-21 223410](https://github.com/user-attachments/assets/5cca681f-d165-49fe-abd0-35ef7a5343bd)


# RESULT
Thus the program for creating a database using ORM hass been executed successfully
