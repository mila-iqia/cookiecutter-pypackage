
Mila Cookiecutter PyPackage
===========================

.. raw:: html

   <img src="https://mila.quebec/wp-content/uploads/2019/12/mila-purple.png" height="120px" align="right">
   <br>

..
.. .. image:: https://pyup.io/repos/github/mila-iqia/cookiecutter-pypackage/shield.svg
..      :target: https://pyup.io/repos/github/mila-iqia/cookiecutter-pypackage/
..      :alt: Updates
..
.. .. image:: https://travis-ci.org/mila-iqia/cookiecutter-pypackage.svg?branch=master
..     :target: https://travis-ci.org/mila-iqia/cookiecutter-pypackage

Cookiecutter_ template for a Python package.

* GitHub repo: https://github.com/mila-iqia/cookiecutter-pypackage/
* Documentation: https://cookiecutter-pypackage.readthedocs.io/
* Free software: BSD license

Features
--------

* Testing setup with ``unittest`` and ``python setup.py test`` or ``pytest``
* Travis-CI_: Ready for Travis Continuous Integration testing
* Tox_ testing: Setup to easily test for Python 3.5, 3.6, 3.7, 3.8
* Sphinx_ docs: Documentation ready for generation with, for example, `Read the Docs`_
* bump2version_: Pre-configured version bumping with a single command
* Auto-release to PyPI_ when you push a new tag to master (optional)
* Command line interface using Click (optional)

.. _Cookiecutter: https://github.com/mila-iqia/cookiecutter

.. Build Status
.. -------------
..
.. Linux:
..
.. .. image:: https://img.shields.io/travis/mila-iqia/cookiecutter-pypackage.svg
..     :target: https://travis-ci.org/mila-iqia/cookiecutter-pypackage
..     :alt: Linux build status on Travis CI
..
.. Windows:
..
.. .. image:: https://ci.appveyor.com/api/projects/status/github/mila-iqia/cookiecutter-pypackage?branch=master&svg=true
..     :target: https://ci.appveyor.com/project/mila-iqia/cookiecutter-pypackage/branch/master
..     :alt: Windows build status on Appveyor

Quickstart
----------

Install the latest Cookiecutter if you haven't installed it yet (this requires
Cookiecutter 1.4.0 or higher)::

    pip install -U cookiecutter

Generate a Python package project::

    cookiecutter https://github.com/mila-iqia/cookiecutter-pypackage.git

Then:

* Create a repo and put it there.
* Add the repo to your Travis-CI_ account.
* Install the dev requirements into a virtualenv. (``pip install -r requirements_dev.txt``)
* Register_ your project with PyPI.
* Run the Travis CLI command `travis encrypt --add deploy.password` to encrypt your PyPI password in Travis configuration.
  and activate automated deployment on PyPI when you push a new tag to master branch.
* Add the repo to your `Read the Docs`_ account + turn on the Read the Docs service hook.
* Release your package by pushing a new tag to master.
* Add a `requirements.txt` file that specifies the packages you will need for
  your project and their versions. For more info see the `pip docs for requirements files`_.
* Activate your project on `pyup.io`_.

.. _`pip docs for requirements files`: https://pip.pypa.io/en/stable/user_guide/#requirements-files
.. _Register: https://packaging.python.org/tutorials/packaging-projects/#uploading-the-distribution-archives

For more details, see the `cookiecutter-pypackage tutorial`_.

.. _`cookiecutter-pypackage tutorial`: https://cookiecutter-pypackage.readthedocs.io/en/latest/tutorial.html
