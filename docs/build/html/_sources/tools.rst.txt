Tools
=====

This section describes a full set of tools for clean Python development.

.. note::

   | Of course, the following list is not exhaustive.
   | Also note that alternatives exist, we only provide guidance for a fully covered development pipe but is subject to evolutions !


Mandatory tools
~~~~~~~~~~~~~~~

Text editor
-----------
Use softwares like `Sublime Text <https://www.sublimetext.com/>`_ or `Notepad++ <https://notepad-plus-plus.org/>`_ for basic editing tasks.
For more performances, using an Integrated Development Environment (IDE)
such as `PyCharm <https://www.jetbrains.com/pycharm/>`_ or `VSCode <https://code.visualstudio.com/>`_
will help to increase development speed by automating some tasks and integrating other tools in a common interface.

git
---
git
    `git <https://git-scm.com/>`_ is a popular Version Control System (VCS) that allows, among other features,
    to save the work state and navigate in history.

GitHub / Gitlab
    Central repositories that host the git files.
    Although central repositories can be self-hosted, we prefer to use turnkey solutions such as
    `GitHub <https://github.com/>`_ or `Gitlab <https://gitlab.com/>`_

poetry
------
`Poetry <https://python-poetry.org/>`_ is a modern package manager for Python.
A Python installation (for example at `C:\Program Files\Python310`) manages its python packages through `pip`



pylint
------
`pylint <https://pypi.org/project/pylint/>`_ is code linter for Python. It statically analyses your
code at normalizing

.. code-block:: console

   $ poetry add pylint


pytest
------
`pytest <https://docs.pytest.org/>`_ runs your Python tests together and output a report.

.. code-block:: console

   $ poetry add pytest

black
-----
`black <https://pypi.org/project/black/>`_ formats your Python code.

.. code-block:: console

   $ poetry add black

Blackened code looks the same regardless of the project you're reading.
You will save time and mental energy for more important matters.



Optional tools
~~~~~~~~~~~~~~

mypy
----
`mypy <https://www.mypy-lang.org/>`_ is an optional static type checker for Python.

.. code-block:: console

   $ poetry add mypy

Sphinx
------
`Sphinx <https://www.sphinx-doc.org/>`_  is a Python documentation generator.

.. code-block:: console

   $ poetry add -D sphinx sphinx-autobuild myst-parser

Write your project documentation using reStructuredText or
Markdown syntax, Sphinx builds a beautiful documentation in the form of a static site (HTML, CSS)
that you can open in a web browser or publish as a website (for example on a GitHub Page).


