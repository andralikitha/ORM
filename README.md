# Ex02 Django ORM Web Application
## Date: 01-04-2024
## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).
## Entity Relationship Diagram
![image](https://github.com/andralikitha/ORM/assets/131592130/9967a9b9-a3c6-4e2d-b54c-3b9af6384688)
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
admin.py:

from django.contrib import admin

from .models import Train, TrainAdmin

admin.site.register(Train, TrainAdmin)

models.py:

from django.db import models
from django.contrib import admin
class Train(models.Model):
    Train_code=models.CharField(max_length=20,primary_key=True)
    Train_name=models.CharField(max_length=100)
    start_time=models.TimeField()
    End_time=models.TimeField()
    start_station_code=models.CharField(max_length=20)
    End_station_code=models.CharField(max_length=20)
 
class TrainAdmin(admin.ModelAdmin):
    list_display=('Train_code','Train_name','start_time','End_time','start_station_code','End_station_code')
## OUTPUT
![image](https://github.com/andralikitha/ORM/assets/131592130/d9ef490a-07b9-4b2c-8d95-b9f30e24394b)

![image](https://github.com/andralikitha/ORM/assets/131592130/ef39fd0f-48d5-490c-97fc-465fedd2df67)
## RESULT
Thus the program for creating a database using ORM hass been executed successfully
