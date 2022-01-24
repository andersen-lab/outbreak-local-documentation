Docker Commands
===============

The Docker Compose file for the project contains five services, which are grouped into profiles.
To simplify we've developed a `Makefile <https://github.com/andersen-lab/outbreak.info/blob/master/Makefile>`_.

In order to rebuild the images for any of these commands, subsitute **run** for **build**.

The Makefile contains several commands meant to make life easier:

Clean old images and containers:

.. code-block:: console

    make clean

.. note::

    * Removes all images and stagnant containers
    * Use with caution

Preprocess new sequencing data:

.. code-block:: console

    make run-new-data

.. note::

    * Uses Bjorn to get .fasta and metadata files from a GitHub repo and preprocesses data for downstream use
    * Make sure you've modified the `bjorn config file <>`_ and changed the `docker-compose.yml <>`_ bind parameter

Ingest data into ElasticSearch and then bring the website up:

.. code-block:: console

    make run-ingest

.. note::

    * Ingests preprocessed data into ElasticSearch, and brings up the ElasticSearch database, tornado server, and client side.
    * Will overwrite a prior ElasticSearch index
    * If zipcode visualizations are wanted, .geojson file must be provided prior to this step

Bring the website up without adding or preprocessing data:

.. code-block:: console

    make run-website

.. note::

    * Brings up the ElasticSearch database, tornado server, and client side

Run all the services:

.. code-block:: console

    make run-website

.. note:: 

    * Runs bjorn to preprocess data, ingests data into ElasticSearch, brings up the ElasticSearch database, tornado server, and client side








