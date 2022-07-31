### **Python Django Framework**
For Web development python has frameworks, like-
    * django
    * flask
Why flask?
    * higher job opportunity
    * strong community

Environment Used--
    * Editor - Visual Studio Code
    * Packaging Tool - pipenv

Knowledge Required--
    * Basic Html/CSS/Javascript
    * Git/GitHub - Basic version controlling (for uploading live server like, hiroku). 

Creating a Django project...
    1) Django Setup:
        * Create a folder 'Django' in any directory
        * Open powershell and go to the directory
        * "mkdir helloworld" - create a directory
        * "cd helloworld\" - go to the directory
        * "pipenv install django" - installing Django
        * "pipenv shell" - activate the virtual env
    2) Creat a Project:
        * "django-admin startproject helloworld_project ." - start a django project in current directory. Here dot(.) means current directory
        * "pyhon .\manage.py runserver" - run the project
        * copy the http address and paste it to any webbrower. It'll appear a bydefault django webpage. That means- your django project is successfully created.
    3) Create a main app: (if you want to add something in your webpage)
        * "python manage.py startapp main_app" - create a app named as main_app
        * Then we need to inform our project about the main app. Go to "settings.py" and name "main_app"
        * After that, we have define urls (http adresses). Go to 'urls.py' and -
            > first import 'include' in django.urls
            > then add the path of main app - 'path('', include('main_app.urls'))'
        * create 'urls.py' file into the main_app and add 'urlpatterns' part including header from 'urls.py'located into helloworld_project.
        * Goto the 'view.py' into the main_app and-
            > clear everything
            > add-
                > from django.http import HttpResponse
                > define a 'homeView' module
        * Go to 'urls.py' in main_app and-
            > import views
            > add the homeView module to the path.