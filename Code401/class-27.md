# Read: Class 27
## Django Models
### Reading Questions:
1- Purpose and Basic Structure of Django Models:
Django models are a key component of the Django framework, used for defining the structure and behavior of data stored in a database. They provide an object-relational mapping (ORM) layer, allowing developers to work with databases using Python classes and objects, rather than writing SQL queries directly.
The basic structure of a Django model involves creating a Python class that inherits from the django.db.models.Model base class. Each attribute of the model class represents a field in the corresponding database table. Django provides various field types such as CharField, IntegerField, DateTimeField, ForeignKey, and more, which define the data types and constraints for the fields.

Models can also include methods and properties to encapsulate business logic and perform operations on the data. For example, a model representing a blog post may have methods for retrieving comments or calculating the number of views.

Django models facilitate the creation and management of database schema by automatically generating the necessary SQL queries for creating tables and managing schema changes. They provide features like migrations, which allow for easy modification of the database schema over time without losing data. Models also handle data validation and provide convenient methods for querying and manipulating data.

2- Features and Customization of the Django Admin Interface:
The Django Admin interface is an automatic administrative interface provided by Django. It allows authorized users to manage and interact with the data stored in the application's database without writing custom views or forms. Some primary features of the Django Admin interface include:
a) Automatic CRUD Operations: The Admin interface automatically generates forms and views for creating, reading, updating, and deleting database records based on the models defined in the application.

b) User Authentication and Permissions: The Admin interface integrates with Django's authentication system, allowing control over user access to different models and actions.

c) Customizable Listing and Detail Views: The Admin interface provides a default display of records in a tabular format and allows customization of the list and detail views by modifying the Admin class associated with the model.

d) Filtering, Searching, and Pagination: The interface offers filtering and searching capabilities for records, making it easier to navigate through large datasets. It also supports pagination to display a limited number of records per page.

e) Extensibility: The Admin interface can be extended to add custom views, actions, or validation logic. Custom templates and CSS styles can also be applied to match the project's design.

3- Key Components and Workflow of a Django Application:
The key components of a Django application include:
a) Models: Models define the database structure and behavior using Python classes. They handle data storage, retrieval, and relationships with other models.

b) Views: Views are Python functions or classes that handle HTTP requests and return HTTP responses. They interact with models to fetch or modify data and pass it to templates.

c) Templates: Templates are HTML files mixed with Django template language (DTL) tags. They define how data is rendered and displayed to the user. Views pass data to templates for rendering.

d) URL Configurations: URL configurations map URL patterns to corresponding views. They define the routing logic for the application, determining which view should handle a particular URL.

e) Forms: Forms handle user input and data validation. They can be generated automatically from models or created manually.

f) Static Files: Static files, such as CSS stylesheets and JavaScript files, are stored and served separately from dynamic content. They are used for enhancing the presentation and functionality of web pages.

The workflow of a Django application typically involves a user making an HTTP request, which is routed to a view based on the URL configurations. The view interacts with models to retrieve or modify data and renders the appropriate template with the data. The template combines HTML markup with data using DTL and is returned as an HTTP response to the user's browser.

## Things I want to know more about
