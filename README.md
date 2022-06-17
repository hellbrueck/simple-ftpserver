# simple-ftpserver

We use the docker (alpine ftp server)[https://github.com/delfer/docker-alpine-ftp-server] for the implementation.

	docker run -p 21:21 -p 21000-21010:21000-21010 -e USERS="guest|geust" delfer/alpine-ftp-server
