# {{ cookiecutter.project_name }} #

{{ cookiecutter.description }}


### Dependency Setup ###

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

Install the requirements in `requirements.txt`:
```
pip install -r requirements.txt
```

### Project Settings Setup ###
Create a `conf/settings/local.py` file. You can use the `conf/settings/local.py.tpl` file as a template. The `local.py` file is needed for the project to run. The only lines of code required for local.py is the following:
```
from __future__ import absolute_import
from .defaults import *
```

Run migrations:
```
./manage.py migrate
```
