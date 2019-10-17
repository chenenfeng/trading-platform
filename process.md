## 1. Use virtual environment

mkdir project
virtualenv .
cd project
source bin/activate

in virtual environment, command line: pip install django
then pip freeze to look at the module installed
  
## 2. 
django-admin.py startproject mysite
python manage.py runserver(check localhost:8000)

## 3. 
create app
mysite urls.py should include crypto.urls


## 4.
<div class="container">
    {% block content %}
    {% endblock %}
</div> 
