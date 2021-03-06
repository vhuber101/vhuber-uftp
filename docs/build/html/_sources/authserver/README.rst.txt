Auth Server
***********

The UFTP authentication service (**Auth server**) is a RESTful
service for authenticating users and initiating UFTP transfers. It is indended to be used with a standalone UFTP client and provides access to one or more UFTPD servers.

Besides data transfer via UFTP and data management features like `ls`, the Auth server also provides REST APIs for data sharing and accessing shared data sets.

The Auth server is based on the UNICORE Services Environment, and all of UNICORE's flexible authentication features and security
configuration options are available as well. For example, the Auth server can be deployed behind a UNICORE Gateway, or it can be configured to use Unity for authenticating users.
