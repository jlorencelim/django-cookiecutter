# Django Cookiecutter #

A [cookiecutter](https://github.com/audreyr/cookiecutter) template for creating initial Django project structure quickly.


## Usage ##

Rather than using startproject and then modifying the project structure, get [cookiecutter](https://github.com/audreyr/cookiecutter) to do all the work.

Setup you virtualenv:
```
$ virtualenv --no-site-packages --prompt=”(<virtualenv-display-name>)” env
$ source env/bin/activate
$ pip install cookiecutter
```
or use a virtualenv wrapper:
```
$ mkvirtualenv --no-site-packages <virtualenv-name>
$ pip install cookiecutter
```

Now run it against this repo:
`$ cookiecutter https://github.com/jlorencelim/django-cookiecutter`

You'll be prompted for some values. Provide them, then a Django project will be created for you. For example:
```
Cloning into 'django-cookiecutter'...
remote: Counting objects: 32, done.
remote: Compressing objects: 100% (25/25), done.
remote: Total 32 (delta 1), reused 32 (delta 1), pack-reused 0
Unpacking objects: 100% (32/32), done.
Checking connectivity... done.
project_name [Project Name]: My Django App
repo_name [my_django_app]:
description [A short description of the project.]: My new Django app.
version [0.1.0]:
```

Enter the project and take a look around:
```
$ cd my_django_app/
$ ls
```

Create your empty repo on your favorite version control hosting service, e.g. [github](https://github.com/), [bitbucket](https://bitbucket.org/) and push it there:
```
$ git init
$ git add .
$ git commit -m "Initial commit"
$ git remote add origin git@github.com:jlorencelim/my_django_app.git
$ git push origin master
```
