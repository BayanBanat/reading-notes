# Class 31
# Django REST Framework & Docker

**Reading Questions :**

1.
  Docker containers streamline application development and deployment through three key components:
  
  **Docker Image**: A standalone package containing all application code, runtime, libraries, and settings. It ensures consistency, portability, and isolation.
  
  **Docker Engine**: The core runtime managing containers. It provides resource efficiency, rapid deployment, and automation integration.
  
  **Docker Registry**: Centralized storage for Docker images. Enables versioning, sharing, offline access, and improved security.
  
  By utilizing these components, Docker simplifies the process of creating, distributing, and running applications in a consistent and efficient manner.
  
2. 
  * Install Django : pip install django
  * Create Project: django-admin startproject
  * Create Django App: python manage.py startapp
  * go to the setting.py in the istalled_app add the apps name
  * Define Models:
    
             class Book(models.Model):
                title = models.CharField(max_length=200)
                author = models.ForeignKey('Author', on_delete=models.CASCADE)
            
                def __str__(self):
                    return self.title
    
    * python manage.py makemigrations
    * python manage.py migrate
    * in the admin.py **admin.site.register(Book)**
    * add your new urls 
    * Create Views:
      
          from django.views.generic import Book
          from .models import Book
          
          class book_list(ListView):
              template_name = 'booklost.html'
              model = Book
      
    * Design Templates
    * Run Development Server:python manage.py runserver
        
3. Django is a full-stack web framework used for building traditional web applications, while Django REST framework (DRF) is an extension of Django specifically designed for building Web APIs. DRF introduces serializers for data serialization, has a flexible URL routing system for API endpoints, and supports various response formats like JSON. It enhances Django's authentication and permission systems for API views and offers a browsable API for easy testing. Django is suitable for HTML-based user interfaces, while DRF is ideal for creating API-centric applications and services.


## Things I want to know more about
