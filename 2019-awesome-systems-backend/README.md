# hackoregon_awesome_systems

![PyPI version](https://badge.fury.io/py/2019-awesome-systems-backend.svg) | [![Build Status](https://travis-ci.org/hackoregon/2019-awesome-systems-backend.svg?branch=master)](https://travis-ci.org/hackoregon/2019-awesome-systems-backend)

Cool awesome project about stuff.

# Documentation

The full documentation is at http://hackoregon.github.io/2019-awesome-systems-backend


# Features

> -   TODO (add what your project does)

# Data Sources

This API package in this repo is based on the Data Science work in the following projects:

* [awesomesauce](http://cnn.com)

# Quickstart to install package in your own Django Project (Non-Hack Oregon Workflow)

* Install hackoregon_awesome_systems:  
  `pip install hackoregon_awesome_systems`

* Add subpackages to your `INSTALLED_APPS`:

  ```python
  INSTALLED_APPS = [     
                      ...     
                      'noad',     
                      ...
                    ]
  ```

* Add hackoregon_awesome_systems's URL patterns:

  ```python
  from hackoregon_awesome_systems.noad
  import urls as noad_urls   

  urlpatterns = [     
                  ...     
                  url(r'^', include(noad_urls)),     
                  ...
                ]
  ```

* Setup your database with a matching schema

* Run the project

# Running Tests

This repo uses pytest and pytest-django to run tests.

For project development work, tests will be run in docker container
using the bin/test.sh script:

# Credits

Tools used in rendering this package:

 * [Cookiecutter](https://github.com/audreyr/cookiecutter)
 * [cookiecutter-djangopackage](https://github.com/pydanny/cookiecutter-djangopackage)
