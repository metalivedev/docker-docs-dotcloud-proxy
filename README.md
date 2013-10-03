# Docker docs proxy

This is a simple dotcloud app, with its main and only purpose to forward
http (and https) requests to docker.readthedocs.org

The reason why we need this is that we have incoming https:// links to
our documentation but without terminating the SSL endpoint and having 
browsers connect directly to docker.readthedocs.org with domain docs.docker.io
users get ugly red warnings.. 

By hosting it here we can serve this app with https and proxy it as plain
http requests to rtd

config by thatcher Okt 2 2013
