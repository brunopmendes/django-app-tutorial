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

6. looking at the INSTALLED_APPS setting and creating any necessary database tables according to the database settings in mysite/settings.py
- py manage.py migrate

7. create polls/models.py, add "polls.apps.PollsConfig" in settings.py and run the command:
- py manage.py makemigrations polls
- py manage.py sqlmigrate polls 0001 (to see what will happen)
- py manage.py migrate

3 steps to make model changes:
- Change your models (in models.py).
- Run python manage.py makemigrations to create migrations for those changes
- Run python manage.py migrate to apply those changes to the database.

8. create superuser admin
