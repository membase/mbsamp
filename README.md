mbsamp
=========

membase sampler/profiling tool

See http://www.membase.org for more info on the Membase NoSQL
database.

Requirements
------------

 * Python
 * Safari web browser is required to see the 3D vbucket visualization
 * Other web browsers will work for the other parts of the web UI.

Usage
-----

To get help:

    ./mbsamp -h

In general usage, first, have a membase cluster running at
http://REST_HOST:REST_PORT.  Then...

    ./mbsamp REST_HOST:REST_PORT [WEB_SERVER_PORT]

For example, if membase is running on localhost:

    ./mbsamp

Then, point your web browser at:

    http://127.0.0.1:8011

mbsamp will sample statistics from the membase cluster,
automatically discovering nodes from the initial node
at http://REST_HOST:REST_PORT

mbsamp will provide a web UI for you to view statistics
results at the given WEB_SERVER_PORT

default REST_HOST:REST_PORT is 127.0.0.1:8091

default WEB_SERVER_PORT for the web-based statistics UI is 8011

License
-------

Apache 2.0

Thanks
------

 * jquery (included)
 * simplejson (included)
 * mc_bin_client/memcacheConstants from Dustin Sallings

