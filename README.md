# Ex02 Django ORM Web Application
# Date:25/11/2025
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 cars

# PROGRAM
```
admin.py

from django.contrib import admin
from .models import car,carAdmin


admin.site.register(car,carAdmin)



models.py

from django.db import models
from django.contrib import admin

class car(models.Model):
    Company=models.CharField(max_length=20)
    Model=models.CharField(max_length=20)
    Colour=models.CharField(max_length=20)
    Price=models.IntegerField()
    DOM=models.DateField()

class carAdmin(admin.ModelAdmin):
    list_display=['Company','Model','Colour','Price','DOM']

```
# OUTPUT

<img width="1919" height="1079" alt=<img width="1919" height="1077" alt="Screenshot 2025-11-25 132210" src="https://github.com/user-attachments/assets/6d492616-b803-417a-8924-1182ffec5cb8" />

<img width="1920" height="1080" alt=<img width="1919" height="1079" alt="Screenshot 2025-11-25 132021" src="https://github.com/user-attachments/assets/7d29beb8-5e96-4efd-8973-0aa284cec20c" />

# RESULT
Thus the program for creating a database using ORM hass been executed successfully
