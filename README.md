BitWasp
===

Bitcoin Address 19EkDTAaGWySZv1QsWxyWwYMZpo7jpvPYe

BitWasp is an open source project which aims to lower the barrier of entry for anyone wishing to set up a bitcoin marketplace. Bitwasp is designed to operate independantly of centralized services, and runs it's own bitcoin server to track payments.

BitWasp is not production ready
===

This project is very much under development, and not yet ready for an alpha. Please be aware the project has not yet underdone extensive security testing and the code is liable to change. Please download and test the code by all means, but don't deploy it on a production system (yet).


Installation
===
Pull the project from our repository, and unzip in your document root.
You may need to alter permissions for temporary files, so execute the following:
chmod 777 ./assets/images -R

Create a database on your server, and import the schema.sql file. 

There is no installer, so you need to set up the config files yourself:
./application/config/database.php :
	- This needs your SQL details. 
./application/config/bitwasp.php :
	- This needs your bitcoind JSON-rpc credentials.

To run the bitcoin server, you'll need a bitcoin.conf:

