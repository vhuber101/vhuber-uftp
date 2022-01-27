PyUFTPD
=======

Python implementation of UFTPD.

.. note::
	*Work in progress!*

The Python version will "take over" from the Java implementation of
the server with version **3.0**

.. topic:: Goals

 * every FTP session gets its own Python process
 * fully drop permissions to the current user
 * better Unix integration (profile, variable resolving etc)
