# simple-ftpserver

We use the docker (alpine ftp server)[https://github.com/delfer/docker-alpine-ftp-server] for the implementation.

with rm we always create a new image, so we loose all data on the ftp.

	docker run --rm -p 21:21 -p 21000-21010:21000-21010 -e USERS="ftpuser|ftpuser" delfer/alpine-ftp-server

to test use ftp command line client

	ftp <servername> 
