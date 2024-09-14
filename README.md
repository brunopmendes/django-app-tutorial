# django-app-tutorial

1. install django 
pip install django

2. start a project called mysite
django-admin startproject mysite

3. run server
py mysite/manage.py runserver

4. create an app called polls
py manage.py startapp polls

5. edit polls/views.py
- create a simple view
- create a urls.py in polls/ and configure the content
- configure the global URLconf in the mysite project to include the URLconf defined in polls.urls