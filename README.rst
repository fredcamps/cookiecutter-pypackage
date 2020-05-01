======================
Cookiecutter PyPackage
======================

This project is a fork from the `original cookiecutter-pypackage`_

.. image:: https://pyup.io/repos/github/fredcamps/cookiecutter-pypackage/shield.svg
     :target: https://pyup.io/repos/github/audreyr/cookiecutter-pypackage/
     :alt: Updates

.. image:: https://travis-ci.org/fredcamps/cookiecutter-pypackage.svg?branch=master
    :target: https://travis-ci.org/fredcamps/cookiecutter-pypackage

Cookiecutter_ template for a Python package.

* GitHub repo: https://github.com/fredcamps/cookiecutter-pypackage/
* Documentation: https://cookiecutter-pypackage.readthedocs.io/
* Free software: BSD license

Features
--------
* IDE Features with Python Language Server
* Static Analysis with mypy, dlint
* Deadcode detection with flake8-erradicate
* Auto Imports with importmagic
* Dependency and environment managment with ``pipenv``
* Testing setup with ``unittest`` and ``python setup.py test`` or ``pytest``
* Travis-CI_: Ready for Travis Continuous Integration testing
* Tox_ testing: Setup to easily test for Python 3.5, 3.6, 3.7, 3.8
* Sphinx_ docs: Documentation ready for generation with, for example, `Read the Docs`_
* bump2version_: Pre-configured version bumping with a single command
* Auto-release to PyPI_ when you push a new tag to master (optional)
* Command line interface using Click (optional)

.. _Cookiecutter: https://github.com/audreyr/cookiecutter

Build Status
-------------

Linux:

.. image:: https://img.shields.io/travis/fredcamps/cookiecutter-pypackage.svg
    :target: https://travis-ci.org/fredcamps/cookiecutter-pypackage
    :alt: Linux build status on Travis CI

Quickstart
----------

Generate a Python package project::

    cookiecutter https://github.com/fredcamps/cookiecutter-pypackage.git

Then:

* Create a repo and put it there.
* Add the repo to your Travis-CI_ account.
* Install the dev requirements into a virtualenv. (``pipenv install --dev``)
* Register_ your project with PyPI.
* Run the Travis CLI command `travis encrypt --add deploy.password` to encrypt your PyPI password in Travis config
  and activate automated deployment on PyPI when you push a new tag to master branch.
* Add the repo to your `Read the Docs`_ account + turn on the Read the Docs service hook.
* Release your package by pushing a new tag to master.
* Activate your project on `pyup.io`_.

.. _Register: https://packaging.python.org/tutorials/packaging-projects/#uploading-the-distribution-archives

For more details, see the `cookiecutter-pypackage tutorial`_.

.. _`cookiecutter-pypackage tutorial`: https://cookiecutter-pypackage.readthedocs.io/en/latest/tutorial.html

Not Exactly What You Want?
--------------------------

Don't worry, you have options:

Similar Cookiecutter Templates
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

* `Nekroze/cookiecutter-pypackage`_: A fork of this with a PyTest test runner,
  strict flake8 checking with Travis/Tox, and some docs and `setup.py` differences.

* `tony/cookiecutter-pypackage-pythonic`_: Fork with py2.7+3.3 optimizations.
  Flask/Werkzeug-style test runner, ``_compat`` module and module/doc conventions.
  See ``README.rst`` or the `github comparison view`_ for exhaustive list of
  additions and modifications.

* `ardydedase/cookiecutter-pypackage`_: A fork with separate requirements files rather than a requirements list in the ``setup.py`` file.

* `lgiordani/cookiecutter-pypackage`_: A fork of Cookiecutter that uses Punch_ instead of bump2version_ and with separate requirements files.

* `briggySmalls/cookiecutter-pypackage`_: A fork using Pipenv_ for package management, with linting, formatting and more.

* Also see the `network`_ and `family tree`_ for this repo. (If you find
  anything that should be listed here, please add it and send a pull request!)

Fork This / Create Your Own
~~~~~~~~~~~~~~~~~~~~~~~~~~~

If you have differences in your preferred setup, I encourage you to fork this
to create your own version. Or create your own; it doesn't strictly have to
be a fork.

* Once you have your own version working, add it to the Similar Cookiecutter
  Templates list above with a brief description.

* It's up to you whether or not to rename your fork/own version. Do whatever
  you think sounds good.

Or Submit a Pull Request
~~~~~~~~~~~~~~~~~~~~~~~~

I also accept pull requests on this, if they're small, atomic, and if they
make my own packaging experience better.


.. _Travis-CI: http://travis-ci.org/
.. _Tox: http://testrun.org/tox/
.. _Sphinx: http://sphinx-doc.org/
.. _Read the Docs: https://readthedocs.io/
.. _`pyup.io`: https://pyup.io/
.. _bump2version: https://github.com/c4urself/bump2version
.. _Punch: https://github.com/lgiordani/punch
.. _Pipenv: https://pipenv.readthedocs.io/en/latest/
.. _PyPi: https://pypi.python.org/pypi

.. _`original cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage/
.. _`Nekroze/cookiecutter-pypackage`: https://github.com/Nekroze/cookiecutter-pypackage
.. _`tony/cookiecutter-pypackage-pythonic`: https://github.com/tony/cookiecutter-pypackage-pythonic
.. _`ardydedase/cookiecutter-pypackage`: https://github.com/ardydedase/cookiecutter-pypackage
.. _`lgiordani/cookiecutter-pypackage`: https://github.com/lgiordani/cookiecutter-pypackage
.. _`briggySmalls/cookiecutter-pypackage`: https://github.com/briggySmalls/cookiecutter-pypackage
.. _github comparison view: https://github.com/tony/cookiecutter-pypackage-pythonic/compare/audreyr:master...master
.. _`network`: https://github.com/audreyr/cookiecutter-pypackage/network
.. _`family tree`: https://github.com/audreyr/cookiecutter-pypackage/network/members
