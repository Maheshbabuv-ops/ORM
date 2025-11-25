# Ex01 Django ORM Web Application
## Date:24/11/2025 

## AIM
To develop a Django application to store and retrieve data from a Car Inventory Database using Object Relational Mapping(ORM).

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
Model.py
```
from django.db import models
from django.contrib import admin
class car(models.Model):
    reg=models.CharField(max_length=20,help_text="car ID")
    car=models.CharField(max_length=100)
    price=models.IntegerField()
    year=models.IntegerField()
class carAdmin(admin.ModelAdmin):
    list_display=('reg','car','price','year')
admin.py
from django.contrib import admin
from .models import car,carAdmin
admin.site.register(car,carAdmin)

```




## OUTPUT
<img width="1906" height="781" alt="Screenshot 2025-11-24 143319" src="https://github.com/user-attachments/assets/1464c23f-c6b0-47a6-ba14-ddddc23452ab" />



## RESULT
Thus the program for creating car inventory database database using ORM hass been executed successfully
