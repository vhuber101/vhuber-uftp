.. _auth-server-building:

Building packages 
=================

You need Java 8 and Apache Maven.

The java code is then built and tested using

.. code:: bash

	mvn install


Creating distribution packages
------------------------------

The following commands create the distribution packages
in tgz, deb and rpm formats


tgz
~~~

.. code:: bash

	mvn package -DskipTests -Ppackman -Dpackage.type=bin.tar.gz


deb
~~~

.. code:: bash

	mvn package -DskipTests -Ppackman -Dpackage.type=deb -Ddistribution=Debian


rpm
~~~

.. code:: bash

	mvn package -DskipTests -Ppackman -Dpackage.type=rpm -Ddistribution=RedHat



