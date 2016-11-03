# {{ cookiecutter.project_name }}


## Requirements

To run this project you need the Docker engine (>=1.12.1) and the docker-compose command (>=1.8.0) installed.

To install the Docker engine on your platform see:

    https://docs.docker.com/engine/getstarted/step_one/

To install docker-compose command:

    https://docs.docker.com/compose/install/


## Getting Started

To start the {{ cookiecutter.project_name }} project run this command from the root folder:

    $ docker-compose up

Migration and a user are needed so run:

    $ docker-compose run django python django-{{ cookiecutter.app_name }}/manage.py migrate
    $ docker-compose run django python django-{{ cookiecutter.app_name }}/manage.py createsuperuser

Now visit [http://localhost:8000/](http://localhost:8000/) to see the application running.

Documentation is served at [http://localhost:9000](http://localhost:9000)
A frontend to the mailhog smtp service is served at: [http://localhost:8025](http://localhost:8025)


## Running the tests

To run the tests:

    $ docker-compose -f containers/test.yml up
