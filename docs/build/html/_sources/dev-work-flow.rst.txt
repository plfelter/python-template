Development flow
================

Documentation
-------------

The full Sphinx documentation creation tutorial is available at https://www.sphinx-doc.org/en/master/tutorial/index.html

Find below a summary of useful commands.


Install Sphinx
~~~~~~~~~~~~~~

Install Sphinx like described in the :ref:`Tools:Sphinx` section.


Init project files (structure and content)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Sphinx provides a utility to easily setup a project:

.. code-block:: console

      $ poetry run sphinx-quickstart docs

      > Separate source and build directories (y/n) [n]: Write “y” (without quotes) and press Enter.
      > Project name: Write “Lumache” (without quotes) and press Enter.
      > Author name(s): Write “Graziella” (without quotes) and press Enter.
      > Project release []: Write “0.1” (without quotes) and press Enter.
      > Project language [en]: Leave it empty (the default, English) and press Enter.



Work on documentation content
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Use any file editor to create and modify .rst or .md files in the /docs/source directory.

* Manual pipe for documentation build after editing

.. code-block:: console

   $ poetry run sphinx-build -b html docs/source/ docs/build/html
   $ poetry run python -m http.server -d ./docs/build/html


* Automatized pipe for concurrent documentation editing and building

.. code-block:: console

   $ poetry run sphinx-autobuild -a -E -b html docs/source/ docs/build/html


Publish as a static website
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Sphinx documentation gives some hints on publishing the static website on ReadTheDocs or
GitHub/Gitlab pages: https://www.sphinx-doc.org/en/master/tutorial/deploying.html
This uses the remote server abilities to build the documentation from the source code.

An alternative is to build the static website on your computer using ``sphinx-autobuild``.


Generate a PDF document
~~~~~~~~~~~~~~~~~~~~~~~

.. code-block:: console

   $ poetry run sphinx-build -M latexpdf docs/source/ docs/build/html




.. note::

   Description of the project work once set up
