Installation
============

.. _clone the repository:

Clone the Repository
--------------------

To install outbreak.info local first clone the repository from GitHub.

.. code-block:: console

    git clone https://github.com/andersen-lab/outbreak.info.git


Outbreak local contains two submodules bjorn and outbreak-api-lite.
Make sure the submodules are populated by navigating to the appropriate folders and running the following:

.. code-block:: console

    git submodule update --init --recursive 

Modify the Configuration Files
------------------------------

Outbreak local uses two different configuration files, one for bjorn and one for the website.
The bjorn config file is located here: 

.. code-block:: console

    /bjorn/example_config.json

For full bjorn documentation, please reference: https://github.com/andersen-lab/bjorn

The website config file is located here:

.. code-block:: console
    /web/src/localConfig.json

Definitions of the parameters in these files can be found under :doc:`parameters`.
