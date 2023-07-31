# Class 34
## API Deployment
**Reading Questions :**
1. **key principles for organizing and configuring Django settings in a project:**

      * Separate Concerns: Divide settings into different files based on their purpose (e.g., base.py, development.py, production.py).
      * Use Environment Variables: Store sensitive information in environment variables, not directly in settings files.
      * Package Usage: Utilize packages like django-environ or python-decouple to manage environment-specific settings.
      * Default Settings: Define default settings in base.py, allow environment-specific files to override them.
      * Avoid Hardcoding: Minimize absolute path hardcoding; use Django-specific variables for dynamic paths.
      * Secrets Handling: Keep secrets secure, avoid exposing them in settings.
      * Security and Debugging: Set DEBUG to False in production, configure ALLOWED_HOSTS properly.
      * Static and Media Files: Configure settings for handling static and media files.
      * Installed Apps: Keep INSTALLED_APPS clean and relevant.
      * Database Configuration: Configure databases based on the environment.
      * Logging Configuration: Set up logging appropriately for different environments.
      * Caching: Use caching to improve performance and set up caching settings.
      * Internationalization and Localization: Configure language and timezone settings.
      * Version Control: Keep settings files under version control.
      * Documentation: Comment settings thoroughly for better understanding.
2. WhiteNoise is a library that enhances the efficient serving of static files in a Django application, particularly in production. It simplifies configuration, handles compression and caching, and eliminates the need for a separate static file server. To integrate WhiteNoise into a Django project:

                  pip install WhiteNoise.
   
                 # Update settings.py:
   
                  Add 'whitenoise.middleware.WhiteNoiseMiddleware' to MIDDLEWARE.
   
                  Set STATICFILES_STORAGE to 'whitenoise.storage.CompressedManifestStaticFilesStorage'.
   
3. Cross-Origin Resource Sharing (CORS) is a security feature that controls access to resources in web applications by preventing unauthorized cross-origin requests. In a Django project, CORS can be implemented and configured using the following steps:

                pip install django-cors-headers 
                
                Add 'corsheaders.middleware.CorsMiddleware' to the MIDDLEWARE setting in settings.py.
                
                Configure allowed origins with the CORS_ALLOWED_ORIGINS setting, specifying the domains allowed to make cross-origin requests.
                
## Things I want to know more about                
  * CORS
  * Django Settings Best Practices
