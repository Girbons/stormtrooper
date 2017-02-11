============
Stormtrooper
============

If `Django`_ + `Wagtail`_ is your first choice for the conquest of the Internet, you need something that spawns quickly your
Django applications!

Getting started
---------------

The Internet is your target; start spawning your first expendable stormtrooper:

.. code-block:: bash

    $ mktmpenv
    $ pip install cookiecutter
    $ cookiecutter https://github.com/girbons/stormtrooper

    # it outputs
    Cloning into 'stormtrooper'...
    remote: Counting objects: 83, done.
    remote: Compressing objects: 100% (52/52), done.
    remote: Total 83 (delta 34), reused 70 (delta 23), pack-reused 0
    Unpacking objects: 100% (83/83), done.
    Checking connectivity... done.

Now you should give a name to your stormtrooper. Wait it's a stormtrooper, they don't have a name.

.. code-block:: bash

    project_name [Storm Trooper]: django
    app_name [stormtrooper]: stormtrooper

The assault checklist
---------------------

1. Add a proper license in the ``LICENSE`` file
2. Add authors and/or contributors in the ``AUTHORS`` file
3. Configure `NewRelic`_ monitoring service
4. Configure `Sentry`_ crash reporting service
5. Use ``pip-tools`` with the ``requirements/requirements.in`` file
6. Check (and update) the ``README.rst`` file present in the newly created app
7. Add the project to your CI (a fake test is already available)
8. Start coding. Really. Start coding now and not before this step!

.. _NewRelic: https://newrelic.com/
.. _Sentry: https://getsentry.com/

Docker
~~~~~~~~

1. Start your app with ``docker-compose up``

License
-------

``Stormtrooper`` is released under the terms of the **BSD license**. Full details in ``LICENSE`` file.

.. _Django: https://www.djangoproject.com/
.. _Wagtail: https://wagtail.io/

Credits
-------

* `Django-wheelie`_ Integration between Wheelie and Django
.. _Django-wheelie: https://github.com/palazzem/django-wheelie

* `Cookiecutter`_ for template spawning!

.. _Cookiecutter: https://github.com/audreyr/cookiecutter
