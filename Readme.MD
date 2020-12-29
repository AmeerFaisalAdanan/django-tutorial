manage.py: a shortcut to use the django-admin command-line utility. It’s used to run management commands related to our project. We will use it to run the development server, run tests, create migrations and much more.


__init__.py: this empty file tells Python that this folder is a Python package.

settings.py: this file contains all the project’s configuration. We will refer to this file all the time!


urls.py: this file is responsible for mapping the routes and paths in our project. For example, if you want to show something in the URL /about/, you have to map it here first.


wsgi.py: this file is a simple gateway interface used for deployment. You don’t have to bother about it. Just let it be for now.


python manage.py runserver - run django webserver

app: is a Web application that does something. An app usually is composed of a set of models (database tables), views, templates, tests.

-- Inside and app it contain 

        migrations/: here Django store some files to keep track of the changes you create in the models.py file, so to keep the database and the models.py synchronized.
        admin.py: this is a configuration file for a built-in Django app called Django Admin.
        apps.py: this is a configuration file of the app itself.
        models.py: here is where we define the entities of our Web application. The models are translated automatically by Django into database tables.
        tests.py: this file is used to write unit tests for the app.
        views.py: this is the file where we handle the request/response cycle of our Web application.



project: is a collection of configurations and apps. One project can be composed of multiple apps, or a single app.
It’s important to note that you can’t run a Django app without a project. Simple websites like a blog can be written entirely inside a single app, which could be named blog or weblog for example.


