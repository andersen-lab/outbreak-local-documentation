Getting Started
===============

Installation
------------

Clone The Repository
^^^^^^^^^^^^^^^^^^^^

To install outbreak.info local first clone the repository from GitHub.

.. code-block:: console

    git clone https://github.com/andersen-lab/outbreak.info.git

Populate the Submodules
^^^^^^^^^^^^^^^^^^^^^^^

Outbreak local contains two submodules bjorn and outbreak-api-lite.
Make sure the submodules are populated by navigating to the appropriate folders and running the following:

.. code-block:: console

    git submodule update --init --recursive

Formatting Data
---------------

All data needs to be appropriately formatted including:

1. Github repository structure for .fasta files and associated metadata.
2. Zipcode .geojson file if provided.

The :doc:`parameters-and-data-formatting` describes these formats in detail.

Modify Parameter Configuration
------------------------------

Two parameter configuration files exist within outbreak.info local.

1. Example parameters for running Bjorn are located `here <https://github.com/andersen-lab/outbreak.info/blob/master/web/src/localConfig.json>`_.
2. Example arameters for everything else are located `here <ihttps://github.com/andersen-lab/bjorn/blob/main/example_config.json>`_.

Prior to executing any commands, these files will need to be filled out appropriately.
The :doc:`parameters-and-data-formatting` section describes each value in detail. 


Run a Docker Command
--------------------
