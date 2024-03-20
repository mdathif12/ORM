# Ex02 Django ORM Web Application
## Date: 18/3/24

## AIM
To develop a Django application to store and retrieve data from a railway database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![image](https://github.com/mdathif12/ORM/assets/149365313/df831b24-a9c1-4647-89fb-4dc1908b3fba)


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
from .models import railway,railwayAdmin
admin.site.register(railway,railwayAdmin)

models.py
from django.db import models
from django.contrib import admin
class railway (models.Model):
    train_code=models.CharField(max_length=20,help_text="railway train_code")
    train_name=models.CharField(max_length=100)
    start_time=models.IntegerField()
    End_time=models.IntegerField()
    start_station_code=models.IntegerField()
    end_station_code=models.IntegerField()
     
class railwayAdmin(admin.ModelAdmin):
    list_display=('train_code','train_name','start_time','End_time','start_station_code','end_station_code',)
```

## OUTPUT

![image](https://github.com/mdathif12/ORM/assets/149365313/09a8d644-bc73-444f-a344-39c5a55c8c90)





## RESULT
Thus the program for creating a database using ORM hass been executed successfully
