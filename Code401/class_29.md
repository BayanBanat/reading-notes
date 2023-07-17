# Read: Class 29
# Django Custom User

**Reading Questions :**
1. The key benefits of using a Django Custom User Model compared to the default Django User Model are:

    * Flexibility: You have full control over the fields and behavior of the user model, allowing customization to fit your application's specific needs.
    * Scalability: You can add or remove fields as your project evolves, ensuring the user model accommodates future requirements.
    * Improved Data Integrity: Enforce data integrity constraints and validation rules to maintain accurate and consistent user data.
    * Enhanced Security: Implement alternative authentication methods, such as email-based or OAuth, to strengthen application security.
    * Easier Integration with Third-Party Apps: Seamlessly integrate with third-party Django apps that expect a specific user model structure.
    * Future Compatibility: Avoid compatibility issues with future Django updates by creating a Custom User Model.

2.
**Step 1: Create a new Django app (if not already created):**

Open your terminal or command prompt.

Navigate to your Django project directory.

Run the command: python manage.py startapp myapp (Replace myapp with the desired name of your app).

**Step 2: Define the Custom User Model:**

Open the models.py file in your app directory.

Import the necessary modules: from django.contrib.auth.models import AbstractBaseUser, BaseUserManager

Create a class for your Custom User Model that inherits from AbstractBaseUser and BaseUserManager.

Define the required fields for your user model. Typically, you would include fields like email, first_name, last_name, etc.

Implement any additional methods or customizations you need for your user model.

**Step 3: Customize the User Manager:**

Inside the same models.py file, create a class for your user manager that inherits from BaseUserManager.

Override the necessary methods such as create_user() and create_superuser().

Implement the logic for creating and managing users.

**Step 4: Update settings.py:**

Open the settings.py file in your project directory.

Find the AUTH_USER_MODEL setting and set it to your Custom User Model's app label and class name, e.g. 'myapp.MyCustomUser'.

**Step 5: Create and apply migrations:**

In your terminal or command prompt, run the command: python manage.py makemigrations to create the initial migrations for your app.

Run the command: python manage.py migrate to apply the migrations and update the database.

**Step 6: Update other references to the User model:**

Search for any references to the default Django User Model (django.contrib.auth.models.User) in your project and update them to use your Custom User Model instead.

**Step 7: Use the Custom User Model:**

You can now use your Custom User Model for authentication, authorization, and any other user-related operations in your Django project.

Access the Custom User Model by importing it where needed: from myapp.models import MyCustomUser.


3. DjangoX is a Django starter framework that enhances Django by providing a preconfigured project structure, settings, authentication system, frontend integration, and development tools. It simplifies project setup and accelerates development, allowing developers to focus on project-specific features. By incorporating DjangoX, developers save time and effort while benefiting from best practices and commonly used functionalities. It is particularly useful when starting a new Django project and needing quick setup and integration of essential components.

    * Example Use Case: Suppose you are starting a new Django project and want to set up the project structure, configure commonly used settings, implement user authentication, and integrate frontend libraries quickly. Instead of starting from scratch and configuring each aspect manually, you can incorporate DjangoX into your project.

## Things I want to know more about
DjangoX
