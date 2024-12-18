# Ex02 Django ORM Web Application
# Date:19/10/2024
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
```python
models.py:
from django.db import models
from django.contrib import admin
class bankloan(models.Model):
    Name=models.CharField(max_length=100)
    Accountno=models.IntegerField(primary_key="Accountno")
    Startdate=models.DateField()
    Email=models.EmailField()
    Mobilenumber=models.IntegerField()
    Amount=models.IntegerField()

class bankloanAdmin(admin.ModelAdmin):
    list_display=('Name','Accountno','Startdate','Email','Mobilenumber','Amount')

admin.py:
from django.contrib import admin
from .models import bankloan,bankloanAdmin
admin.site.register(bankloan,bankloanAdmin)
```
# OUTPUT
![imgggg](https://github.com/user-attachments/assets/8340a9fd-c90c-45cd-9411-88dc9a718971)

![Screenshot 2024-12-09 150556](https://github.com/user-attachments/assets/f6081686-a3d9-4364-9002-4d8ee69dbb89)

![Screenshot 2024-12-09 151024](https://github.com/user-attachments/assets/153fad17-fa52-401f-bf44-9c8690fea747)

![Screenshot 2024-12-12 133102](https://github.com/user-attachments/assets/ce700f1e-20b3-433f-bf8f-85181aeadb8a)


# RESULT
Thus the program for creating a database using ORM hass been executed successfully
