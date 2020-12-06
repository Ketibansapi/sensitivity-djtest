[![Build Status](https://travis-ci.org/nocarryr/django-safe-project.svg?branch=master)](https://travis-ci.org/nocarryr/django-safe-project)

# sensitivity-djtest-project
Create a system that is able to save files and analyze the files’ sensitivity score.

## Installation
To install `sensitivity-djtest-project` run:
```
pip install django-safe-project
```

## Usage

When installed, call
```
django-safe-project <projectname>
```
instead of
```
django-admin startproject <projectname>
```

This will create a separate module in the project path named `local_settings.py` containing all the things you don't want to ever place in any sort of VCS ever.

`local_settings.py` will then be gitignored and its contents imported into the main `settings.py` module.

Currently the list of settings this handles are:

* SECRET_KEY
* DATABASES
* DEBUG
* ALLOWED_HOSTS
