Interact With Actors
====================

In Tapis, actors are container-based functions-as-a-service that follow the actor model of concurrent computation. An actor responds to messages it receives by changing its state, performing an action, sending out response messages, or all of the above.

The function an actor performs is exposed as the default command in a container. It is typically quick and requires little processing power - i.e. an app may be configured to run FastQC, and an actor may trigger a job using that app.

The guide below is a brief introduction to interacting with actors on the Tapis platform.


**Prerequisite**
    - Install tapis-cli

The following command throws a help text of the available actors commands available.

.. code-block:: bash

  $ tapis actors -h
    Command "actors" matches:
    actors aliases create
    actors aliases delete
    actors aliases list
    actors aliases show
    actors create
    actors delete
    actors deploy
    actors execs list
    actors execs logs
    actors execs show
    actors list
    actors nonces create
    actors nonces delete
    actors nonces list
    actors nonces show
    actors pems grant
    actors pems list
    actors pems revoke
    actors pems show
    actors run
    actors show
    actors submit
    actors update
    actors workers create
    actors workers delete
    actors workers list
    actors workers show

Working with an Actor command
-----------------------------
.. code-block:: bash

   $ tapis actors list
