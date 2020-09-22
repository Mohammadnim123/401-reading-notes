# Django Custom User Model

Django ships with a built-in User model for authentication, however the official Django documentation highly recommends using a custom user model for new projects. The reason is if you want to make any changes to the User model down the road--for example adding a date of birth field--using a custom user model from the beginning makes this quite easy. But if you do not, updating the default User model in an existing Django project is very, very challenging.

So always use a custom user model for all new Django projects. However the official documentation example is not actually what many Django experts recommend using. There is a far easier yet still powerful approach to starting off new Django projects with a custom user model which I'll demonstrate here.

If you're brand new to user authentication in Django, I recommend first reviewing how to implement a regular login, logout, signup flow in Django which covers the basics in detail.

**Setup**

To start, create a new Django project from the command line. We need to do several things:

* create and navigate into a dedicated directory called accounts for our code
* install Django
* make a new Django project called config
* make a new app accounts
* start the local web server

**Here are the commands to run:**

1. $ cd ~/Desktop
1. $ mkdir accounts && cd accounts
1. $ pipenv install django~=3.1.0
1. $ pipenv shell
1. $ django-admin.py startproject config .
1. $ python manage.py startapp accounts
1. $ python manage.py runserver

>Note that we did not run migrate to configure our database. It's important to wait until after we've created our new custom user model before doing so.

**AbstractUser vs AbstractBaseUser**

There are two modern ways to create a custom user model in Django: AbstractUser and AbstractBaseUser. In both cases we can subclass them to extend existing functionality however AbstractBaseUser requires much, much more work. Seriously, don't mess with it unless you really know what you're doing.

>Now that our custom user model is configured you can easily and at any time add additional fields to it. See the Django docs for further instructions.

>You can also check out DjangoX, which is an open-source Django starter framework that includes a custom user model, email/password by default instead of username/email/password, social authentication, and more.
