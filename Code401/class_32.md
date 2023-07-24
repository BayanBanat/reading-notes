# Class 32
# Permissions & Postgresql
**Reading Questions :**
1. Django Rest Framework (DRF) provides a powerful set of permissions for securing an API. **The key components include:**

   * Authentication: DRF offers various authentication classes (e.g., BasicAuthentication, TokenAuthentication) to verify user identity before granting access to protected views.
    
   * Authorization: DRF permissions define rules for user actions (e.g., read, write) on specific resources or endpoints. They ensure that only authorized users can perform certain actions.
    
   * Built-in Permission Classes: DRF provides ready-to-use permission classes like AllowAny, IsAuthenticated, and IsAdminUser, offering different levels of access control.
    
   * Custom Permission Classes: DRF allows you to create custom permission classes tailored to your application's needs, enabling fine-grained access control.
2. In SQL, the SELECT statement is used to retrieve data from a database table. It allows you to specify which columns or expressions you want to retrieve, as well as any filtering or sorting criteria.

     **The basic syntax of the SELECT statement is as follows:**
   
            SELECT column1, column2, ... 
            FROM table_name;
   
    **To retrieve all columns from a table called 'employees**
   
             SELECT *
             FROM employees;

4. The role of DRF Generic Views is to simplify the development of RESTful APIs in Django Rest Framework (DRF). These pre-built view classes encapsulate common patterns for handling various API operations, such as creating, retrieving, updating, and deleting data.
        from django.shortcuts import render
        from .models import Snack
        from rest_framework.generics import ListCreateAPIView,RetrieveUpdateDestroyAPIView
        from .serializers import SnackSerializer
        
        class SnackListView(ListCreateAPIView):
        
            queryset = Snack.objects.all()
            serializer_class = SnackSerializer
        
        
        class SnackDetailView(RetrieveUpdateDestroyAPIView):
            queryset = Snack.objects.all()
            serializer_class = SnackSerializer


## Things I want to know more about
  DRF Permissions

 

