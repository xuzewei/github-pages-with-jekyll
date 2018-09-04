---
title: "Install Wordpress on Docker"
date: 2018-09-04
---
# docker-wordpress-workflow

## Install wordpress/mysql/phpadmin on docker

```sh
$ docker-compose up -d
```

## Confrence

### Installing Docker on Ubuntu 18.04

On Ubuntu 18.04, installing Docker is achieved in three lines of bash commands at most. 

installation:

```sh
$ sudo apt-get update
$ sudo apt-get install -y wget
$ sudo wget -qO- https://get.docker.com/ | sh

#You can test that the installation worked fine by checking the version of Docker:
$ sudo docker --version

#You can stop, start, and restart the service. For example, to restart it:
$ sudo service docker restart

#If you want to use docker from a nonroot user, add the user account to the docker group. When it's done, exit the current shell and log in again or start a new shell for the
change to take effect.
$ sudo gpasswd -a <user> docker
```

### Install Docker Compose on Ubuntu 18.04

Use Docker Compose, a command-line utility to define and run multicontainer applications with Docker. With Compose, you define the services that need to run in a YAML file. 

```sh
$ sudo apt-get install python-pip
$ sudo pip install -U docker-compose
```

Or via curl:
```sh
$ curl -L https://github.com/docker/compose/releases/download/1.4.0/\
 docker-compose-`uname -s`-`uname -m` > /usr/local/bin/docker-compose
```

