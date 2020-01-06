
MyModule
========

Sample Python module.
Just clone this repository and change all `mymodule` to your module name. Also search for `python_module` because it's used in some URLs that point to the repository.

Suppose you want to create a new Python library called `yourmodule`.
You can use the next GNU/Linux commands inside the repository folder:

    # Search and replace mymodule by your module name.
    find . -not -path '*/\.*' -type f -exec sed -i 's/mymodule/yourmodule/g' {} +
    # Sometimes is written in upper case (mainly in docs).
    find . -not -path '*/\.*' -type f -exec sed -i 's/MyModule/YourModule/g' {} +
    # Search and replace python_module by your repository name.
    find . -not -path '*/\.*' -type f -exec sed -i 's/python_module/yourmodule/g' {} +
    # Rename the module folder
    mv mymodule yourmodule


Getting started
---------------

These instructions will get you a copy of the project up and running on your local machine.


### Prerequisites

The minimum Python version supported is version 3.


### Install

Install the package in a dev environment with:

    python setup.py develop

This line will automatically install all the dependencies.


## Upload module to PyPi

Generate dist files:

    python setup.py sdist bdist_wheel

Upload the generated files with Twine using your PyPi account:

    python -m twine upload dist/*


## Running the tests

Run the automated tests with:

    python -m pytest


Contributing
------------

Please read [CONTRIBUTING.md](https://github.com/guiferviz/python_module/blob/master/CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests.


Versioning
----------

We use [SemVer](http://semver.org/) for versioning.


Authors
-------

List of main contributors:

* **Guille** - [guiferviz](https://github.com/guiferviz)

For a full list of contributors see [AUTHORS](https://github.com/guiferviz/python_module/blob/master/AUTHORS.md).


License
-------

This project is licensed under the **MIT License**, see the [LICENSE](https://github.com/guiferviz/python_module/blob/master/LICENSE) file for details.


Acknowledgments
---------------

 * Attribution to anyone whose code was used.
 * You've been inpired by...
 * Say thanks to someone.
