# Read: Class 28
# Django CRUD and Forms
**Reading Questions:**
1. To create a form using Django, you need to define a form class that inherits from the django.forms.Form class. Here are the key components and steps involved:
  * Import the necessary modules: Start by importing the required modules. Typically, you'll need to import django.forms.
  * Create a form class: Define a form class that inherits from django.forms.Form. This class represents the form and contains fields and validation rules.
  * Define form fields: Inside the form class, define various fields using field classes such as CharField, EmailField, IntegerField, etc. Each field represents an input element in the form.
  * Define field attributes: Specify various attributes for each field, such as label text, help text, placeholder, initial value, required status, validation rules, etc. These attributes control how the field is rendered and validated.
  * Handle form submission: In the view function or class-based view, instantiate the form class and pass it to the template context. When the user submits the form, you can process the form data by creating an instance of the form and calling its is_valid() and cleaned_data methods to validate and retrieve the cleaned data.
  * Render the form: In the template, you can render the form fields by accessing them using the dot notation. Django provides template tags and filters to handle form rendering and display validation errors.
  * Display validation errors: If the form data is invalid, Django automatically populates the form with error messages. You can iterate over the form's fields in the template to display these errors.
  * Process form data: Once the form is valid, you can access the cleaned data through the cleaned_data dictionary. You can then process this data as required, such as saving it to a database or performing any necessary actions.
2. Django Templates are used in web development to generate dynamic HTML pages by combining static content with dynamic data. They separate logic and presentation, allowing developers to create reusable and maintainable HTML templates. Template inheritance is a feature of Django Templates that improves code reusability and maintainability. It involves creating a base template with common elements and layout and then creating child templates that inherit from the base template and override or add specific sections. Template inheritance promotes code modularity, reduces duplication, and simplifies maintenance by allowing updates to the base template to automatically propagate to all child templates. It enables teams to work on different sections independently and provides customization flexibility while maintaining a consistent design.
3. Django Views handle requests and generate responses. There are function-based views (FBVs) and class-based views (CBVs). FBVs are functions, while CBVs are classes with built-in features. FBVs offer flexibility, while CBVs provide code reuse and abstraction. Django offers both types for different development needs.



## Things I want to know more about
* Django Forms
* Django Views











