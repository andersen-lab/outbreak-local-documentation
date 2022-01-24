Welcome to Outbreak Local's Documentation!
==========================================

Outbreak.info Local is an offshoot project from `Outbreak.info <https://outbreak.info/>`_, which originated in the Su, Wu, 
and Andersen labs at Scripps Research. The goal of Outbreak.info Local is to allow researchers to use the outbreak.info
visualizations for genomic variants to explore SARS-CoV-2 data from customizable data sources.

Using `tornado <https://www.tornadoweb.org/en/stable/>`_,  and `ElasticSearch <https://www.elastic.co/>`_ users can turn their
sequnces in to a website and api for original data analysis. The process is dockerize to make it as simple as possible.

How it Works Overview
----------------------

.. image:: ../static/flowchart.png
    :class: align-right

1. Sequencing data is pre-proccessed using the tool `bjorn <https://github.com/andersen-lab/bjorn>`
2. Pre-processed data is ingested into ElasticSearch
3. Tornado 
4.
5. 

Check out how to :doc:`install` the project.

.. note::

   This project is under active development.

Contents
--------

.. toctree::

   install
   getting-started
   docker-commands
   parameters
   troubleshooting
