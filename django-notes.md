# Django Notes

To create a new app, use command
> python manage.py startapp app_name

To create a URL mapping for your app, create a separate 'urls.py' file for your app.

Add the templates folder (where you create your html pages) in project's settings.py -> TEMPLATES -> DIRS

If you want the page to be dynamic, pass the variable = value wherever you are defining the view and then refer that variable in the HTML page using two curly brackets {{variable_name}} (Jinga Pattern)

To extend HTML page into another page use
{% extends 'base.html' %}
To put another HTML content in between HTML page use:
{% block content %}

{% endblock %}

Add the form action url in the urls.py and define a view function for that in views.py and render the desired html page

To get a value from the form to your django in view just use requests.get['variable name']

