.. _uftp-client-building:

Building packages for the 'uftp' client
---------------------------------------

You need Java and Apache Maven. 
Check the versions given in the pom.xml file. 

Creating distribution packages
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The following commands create the distribution packages
in tgz, deb and rpm formats. The versions are taken from the pom.xml


tgz
+++

.. code:: bash

	mvn package -DskipTests -Ppackman -Dpackage.type=bin.tar.gz


deb
+++

.. code:: bash

	mvn package -DskipTests -Ppackman -Dpackage.type=deb -Ddistribution=Debian


rpm redhat
++++++++++

.. code:: bash

	mvn package -DskipTests -Ppackman -Dpackage.type=rpm -Ddistribution=RedHat



