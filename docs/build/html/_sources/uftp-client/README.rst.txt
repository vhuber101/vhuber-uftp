UFTP standalone client
**********************

This is a Java-based client for UFTP. It allows to 

 * list remote directories
 * upload/download files
 * sync files
 * make remote directories
 * delete remote files or directories
 * manage shares and access shared data

It supports username/password authentication, token authentication,
and ssh-key (on Linux) authentication to a UFTP Authentication Server
or UNICORE/X server.


.. topic:: Prerequisites

	* Java 8 (OpenJDK, Oracle, IBM)
	
	* Access to a UFTP authentication service and the corresponding UFTPD server. To use the client, you need to know the address of the authentication service.


.. topic:: Installation

	Unzip the archive in a location of your choice. Add the 	'bin'
	directory to your path. (Alternatively, you can copy 	'bin/uftp' script
	to a directory that is already on your path, in this case
	edit the script and setup the required directories.)


.. topic:: Usage

	Invoking ``uftp`` will list the available commands.

	Invoking ``uftp <command> -h`` will show help for a command

	For password authentication, use the "-P" option. The password can be written into the URL, for example:

	.. code:: bash

		$> uftp ls -u demo:password
		https://localhost:9000/rest/auth/TEST:/home/demo/

	If not given on the command line, the password will be queried interactively.

	For detailed usage instructions and examples, refer to the :ref:`uftp-client-manual` available in the doc directory or online.

