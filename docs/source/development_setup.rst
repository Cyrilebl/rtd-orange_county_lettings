Development Setup
=================


Virtual environment
-------------------

In the root of your project, create a `.env` file and add the following variables:

.. code-block:: text

    DEBUG=True
    ALLOWED_HOSTS=localhost
    SECRET_KEY=<secret_key>
    SENTRY_DSN=<sentry_project_url>


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

1. Create an account on `Sentry <https://sentry.io/>`.
2. Add your Sentry project URL to the `.env` file under the `SENTRY_DSN` variable:

.. code-block:: text

   SENTRY_DSN=<sentry_project_url>
