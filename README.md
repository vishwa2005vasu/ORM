# Ex02 Django ORM Web Application
## Date:06/03/2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![Screenshot (219)](![313469473-c1e8d53b-1640-4346-9f10-b5b0919eb9021](https://github.com/vishwa2005vasu/ORM/assets/135954202/9be9b2d3-a881-4c4c-8eb6-84e0d227dc28)
)




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

from django.contrib import admin
from .models import book_DB,book_DBAdmin
admin.site.register(book_DB,book_DBAdmin)

models.py
from django.db import models
from django.contrib import admin
class book_DB(models.Model):
    bookno=models.IntegerField(primary_key=True);
    bookname=models.CharField(max_length=10);
    authorname=models.CharField(max_length=10);
    yearofpublishing=models.DateField();
    pages=models.IntegerField();
    price=models.IntegerField();

class book_DBAdmin(admin.ModelAdmin):
   list_display=("bookno","bookname","authorname","yearofpublishing","pages","price");


```

## OUTPUT
![Screenshot (216)](https://github.com/vishwa2005vasu/ORM/assets/135954202/174164a4-89a4-4391-90dd-f713d5d72023)





## RESULT
Thus the program for creating a database using ORM hass been executed successfully
