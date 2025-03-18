Development setup
=================


.. _virtual_environment:

Virtual environment
-------------------

In the root of your project, create a `.env` file and add the following variables:

.. code-block:: text

    DEBUG=True
    ALLOWED_HOSTS=localhost
    SECRET_KEY=<secret_key>
    SENTRY_DSN=<sentry_url>


.. _linting:

Linting
-------

To check code quality, use `flake8`:

.. code-block:: console

   flake8


.. _unit_tests:

Unit Tests
----------

To run the unit tests, use `pytest`:

.. code-block:: console

   pytest
