# Class 33
## Authentication & Production Server
**Reading Questions :**
1.   *  JSON Web Tokens (JWTs) are a type of token commonly used for authentication and authorization in web applications and APIs. The primary purpose of JWTs is to securely transmit information between parties in a compact and self-contained format. They are often used to represent claims between the parties involved and can be used to authenticate users and to authorize access to specific resources.
     *  They consist of three parts: header, payload (claims), and signature. The header specifies the token type and signing algorithm. The payload contains information (claims) about the user or other data. The signature ensures the token's integrity and authenticity. JWTs are compact, self-contained, and can be used for authentication and authorization. When received, the recipient validates the signature to ensure trust and extracts the claims for further use. Avoid storing sensitive data in JWTs and use encryption for added security.
2. JWT authentication can be integrated with Django REST Framework (DRF) to secure API endpoints. DRF is a powerful toolkit for building Web APIs in Django, and it provides built-in support for various authentication methods, including JWT.

              pip install djangorestframework-simplejwt
   

              # settings.py
                    
                          REST_FRAMEWORK = {
                              'DEFAULT_AUTHENTICATION_CLASSES': [
                                  'rest_framework_simplejwt.authentication.JWTAuthentication',
                              ],
                          }
   
             # urls.py

                                from django.urls import path
                                from rest_framework_simplejwt import views as jwt_views
                                
                                urlpatterns = [
                                    # Your URLs...
                                    path('api/token/', jwt_views.TokenObtainPairView.as_view(), name='token_obtain_pair'),
                                    path('api/token/refresh/', jwt_views.TokenRefreshView.as_view(), name='token_refresh'),
                                ]
   
               # views.py

                            from rest_framework.views import APIView
                            from rest_framework.response import Response
                            from rest_framework.permissions import IsAuthenticated
                            
                            
                            class HelloView(APIView):
                                permission_classes = (IsAuthenticated,)
                            
                                def get(self, request):
                                    content = {'message': 'Hello, World!'}
                                    return Response(content)
   

              # urls.py

                                    from django.urls import path
                                    from myapi.core import views
                                    
                                    urlpatterns = [
                                        path('hello/', views.HelloView.as_view(), name='hello'),
                                    ]
   
                                       
4. Django's built-in development server (runserver) is not suitable for production due to security and performance limitations. It lacks essential features like SSL termination and process management for handling concurrent requests. For deploying a Django application in production, consider using alternative servers like Gunicorn, uWSGI, Daphne, or Hypercorn. Additionally, Nginx or Apache can be used as a reverse proxy in front of the application server to handle tasks like SSL termination and load balancing. Proper configuration and adherence to best practices are crucial for security, performance, and scalability. Docker and container orchestration platforms can simplify deployment and ensure consistency across environments.

## Things I want to know more about   
