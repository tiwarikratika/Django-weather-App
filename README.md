<h2>This repository implements a weather app that uses Open Weather API and Django as a backend framework.</h2>


<h1>Workflow</h1>

The following is a basic workflow that you can use as a quick reference for developing a Django Project.

<h2>Setup<h2>
Within a new directory, create and activate a virtualenv.
Install Django.
  
<li>Create your project:  </li>
  
django-admin.py startproject  


<li>Create a new app</li>
 python manage.py startapp  

 
  
  <li>  Add your app to the INSTALLED_APPS tuple.</li>
  <li>Add Basic URLs and Views</li>
  <li>Map your Project’s urls.py file to the new app.</li>
  <li>In your App directory, create a urls.py file to define your App’s URLs.</li>
<li>Add views, associated with the URLs, in your App’s views.py; make sure they return a HttpResponse object. Depending on the situation, you may also need to query the model (database) to get the required data back requested by the end user.</li>
  
    
    
Templates and Static Files
  <ul>
    <li>Create a templates and static directory within your project root.</li>
    <li>Update settings.py to include the paths to your templates.</li>
    <li>Add a HTML file to the templates directory. </li>
    <li> Update the views.py file as necessary.</li>
  </ul>
  
  
 Models and Databases
  <li>Update the database engine to settings.py (if necessary, as it defaults to SQLite).</li>
  <li>Create and apply a new migration.</li>
  <li>Create a super user.</li>
  <li>Add an admin.py file in each App that you want access to in the Admin.</li>
  <li>Create your models for each App.</li>
  <li>Create and apply a new migration. </li>
  
  
 Forms
  <ul>
<li>Create a forms.py file at the App to define form-related classes; define your ModelForm classes here.</li>
<li>Add or update a view for handling the form logic - e.g., displaying the form, saving the form data, alerting the user about validation errors, etc.</li>
    <li>Add or update a template to display the form.</li>
    <li>Add a urlpattern in the App’s urls.py file for the new view.</li>
    <ul>
  
User Registration
  <ul>
    <li>Create a UserForm</li>
    <li>Add a view for creating a new user.</li>
    <li>Add a template to display the form.</li>
    <li>Add a urlpattern for the new view.</li>
    </ul>
  
 

