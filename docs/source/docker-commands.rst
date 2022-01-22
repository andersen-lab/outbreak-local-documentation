Docker Commands
===============

The Docker Compose file for the project contains five services, each with a container.
To simplify we've developed a Makefile here: https://github.com/andersen-lab/outbreak.info/blob/master/Makefile

The Makefile contains several commands meant to make life easier:

Clean:

.. code-block:: console

    make clean

Removes all images and stagnant containers. Use with caution.

Build-New-Data:

.. code-block:: console

    make build-new-data

Builds the image to create new data from a github repository.

Run-New-Data:

.. code-block:: console

    make run-new-data

Runs the new-data pipeline which uses bjorn to process data. If the image isn't present this command will create it.

Build-Ingest:

.. code-block:: console

    make build-ingest


