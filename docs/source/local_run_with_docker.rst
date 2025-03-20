Local run with Docker
=====================

To start the server locally using Docker Hub image, run the following command:

.. code-block:: console

   docker pull tidebryt/orange-lettings:latest && docker run --env-file .env -p 8000:8000 --name oc-lettings -d tidebryt/orange-lettings:latest

Then, open `http://localhost:8000/` in a web browser.

Managing the Container
----------------------

Use the following commands to manage the Docker container:

- **Stop the container**:  
  
  .. code-block:: console

     docker stop oc-lettings

- **Restart the container**:  

  .. code-block:: console

     docker start oc-lettings
    
- **Remove the container**:  

  .. code-block:: console

     docker rm oc-lettings