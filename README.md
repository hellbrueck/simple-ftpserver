# simple-ftpserver

We use the docker (alpine ftp server)[https://github.com/delfer/docker-alpine-ftp-server] for the implementation.

with option --rm we always create a new image. be aware that we loose all data on the ftp server. use option -d to run detached.	

	docker run --rm -p 21:21 -p 21000-21010:21000-21010 -e USERS="ftpuser|ftpuser" delfer/alpine-ftp-server

to test use ftp command line client

	ftp <servername> 

or winscp with setting ftp

