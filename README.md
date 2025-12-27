# Ex01 Django ORM Web Application
# Date:26/11/2025
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
enter the code for admin.py and model.py


# PROGRAM
```models.py

from django.db import models
from django.contrib import admin
class Product(models.Model):
    Id= models.AutoField(primary_key=True)
    ProductName=models.CharField(max_length=10)
    PBrand=models.CharField(max_length=18)
    Product_MRP=models.CharField(max_length=12)
    PType=models.CharField(max_length=15)
    manuf_date=models.DateField(default="not available")

class ProductAdmin(admin.ModelAdmin):
    list_display=["ProductName","PBrand","Product_MRP","manuf_date"]```
admin.py

from django.contrib import admin
from .models import Product,ProductAdmin
admin.site.register(Product,ProductAdmin)
```

# OUTPUT
<img width="1917" height="1015" alt="Screenshot 2025-11-26 094238" src="https://github.com/user-attachments/assets/82e7e6f8-c85d-45c5-a6de-76a4717a03cd" />



# RESULT
Thus the program for creating a database using ORM hass been executed successfully
