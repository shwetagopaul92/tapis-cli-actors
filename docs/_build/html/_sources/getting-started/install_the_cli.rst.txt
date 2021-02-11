Install the CLI
================

The Tapis CLI is available as a Python package. We highly recommend using Python 3.7+ as the Python runtime behind the Tapis CLI.
We support Python 2.7 for legacy applications, but on a best-effort basis as Python 2.7 is a deprecated language.

Tapis CLI is a human-friendly, scriptable command line interface, implemented in Python, that helps scientists and engineers build and manage scalable computational and data science workflow projects using the Tapis platform.
It is a replacement for a pure-Bash CLI environment known as agave-cli that we hope brings you new features, better reliability, and dramatically enhanced productivity.

Tapis CLI provides a unified interface to multiple web service APIs, allowing them to be easily orchestrated and composed into higher-order constructs combining HPC, data management, cloud computing, and other aspects of computing.

Documentation: <https://tapis-cli.readthedocs.io/en/latest/>

Install with Pip
----------------

.. code-block:: bash

  $ pip install tapis-cli


Install from Source
-------------------

.. code-block:: bash

  $ git clone https://github.com/TACC-Cloud/tapis-cli-ng.git
  $ cd tapis-cli-ng/
  $ pip install --upgrade --user .


Run in a Container
------------------

.. code-block:: bash

  $ docker run --rm -it -v ${PWD}:/work -v ${HOME}/.agave:/root/.agave \
      tacc/tapis-cli-ng:latest /bin/bash
