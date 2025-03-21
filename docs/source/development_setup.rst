Development Setup
=================


Virtual environment
-------------------

In the root of your project, create a `.env` file and add the following variables:

.. code-block:: text

    DEBUG=True
    ALLOWED_HOSTS=localhost
    SECRET_KEY=<secret_key>


Linting
-------

To check code quality, use `flake8`:

.. code-block:: console

   flake8


Unit tests
----------

To run the unit tests, use `pytest`:

.. code-block:: console

   pytest


Coverage
--------

To check the code coverage, use `coverage`:

.. code-block:: console

   coverage run -m pytest
   coverage report


Error monitoring
----------------

The application uses **Sentry** for error and event logging.
Please ask the admin to add you to the Sentry project.
