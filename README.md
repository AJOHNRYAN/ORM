# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django Application to store and retrieve data from a Vehicle Service Database platform using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM



## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Detect changes and create migration files that describe how to modify the database schema

### STEP 5:
Execute the migration files and update the database schema to match your Django models

### STEP 6:
Create a superuser with full access rights to all models and data through the admin interface.

### STEP 7:
Apply the migration files of the created app to the database

### STEP 8:
Execute Django admin using localhost and create details for 10 entries

## PROGRAM
from django.db import models
from django.contrib import admin
class Service(models.Model):
    Vehical_NO=models.CharField(primary_key=True, max_length=100)
    Vehical_Name=models.CharField(max_length=100)
    Name=models.CharField(max_length=100)
    mobile=models.IntegerField()
    Address=models.TextField(max_length=100)
    Fault=models.TextField(max_length=100)
    Billings=models.IntegerField(max_length=10000)
class ServiceAdmin(admin.ModelAdmin):
    list_display = ("Vehical_NO", "Vehical_Name", "Name", "mobile", "Address","Fault","Billings")


## OUTPUT
<img width="1600" height="900" alt="WhatsApp Image 2026-10-12 at 2 03 36 PM" src="https://github.com/user-attachments/assets/e4e2e3b5-f0bb-482f-94ba-22e1750212d9" />



## RESULT
Thus the program for creating Online Food Delivery Database using ORM hass been executed successfully
