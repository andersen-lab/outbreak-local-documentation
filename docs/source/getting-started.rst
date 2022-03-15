Getting Started
===============

Overview
--------

1. Install
2. Format data
3. Modify configuration parameters
4. Run docker command

Installation
------------

Clone The Repository
^^^^^^^^^^^^^^^^^^^^

To install outbreak.network local build first clone the repository from GitHub.

.. code-block:: console

    git clone git@github.com:andersen-lab/outbreak.info.git

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
2. Example parameters for everything else are located `here <ihttps://github.com/andersen-lab/bjorn/blob/main/example_config.json>`_.

Prior to executing any commands, these files will need to be filled out appropriately.
The :doc:`parameters-and-data-formatting` section describes each value in detail. 


Run a Docker Command
--------------------

Each major step (Bjorn, ElasicSearch Ingestion, ElasticSearch, Tornado, and Client) is defined as a service in the `docker-compose.yml <https://github.com/andersen-lab/outbreak.info/blob/master/docker-compose.yml>`_. The `Makefile <https://github.com/andersen-lab/outbreak.info/blob/master/Makefile>`_ allows for easy running of groups of services. Example commands to run Makefile profiles can be found :doc:`docker-commands`.
