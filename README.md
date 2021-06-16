# PHP website on Nginx (Docker-compose)
[![Builds](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

---
# Description

Creating a simple php website using Docker-compose. Website will be self-signed.

---

# Features

- Docker-compose is used for easy deploy.
- You can upload your own php website in the website folder which is 'bind mounted' to the container.

---
# Prerequisites

- Need to have Docker installed in your machine.
- Need to have Git installed in your machine.
- Need to have Docker-compose installed in your machine.

---
# Installation 

- [Docker installation]("https://docs.docker.com/get-docker/") 
- Alternatively from the above, you can use Pre-installed [Docker Terminal]("https://labs.play-with-docker.com/") _(For the easy access to configured Docker environment especially for beginers)
- [Git installation]("https://git-scm.com/download/linux")
-  [Docker-compose](https://docs.docker.com/compose/install/)

---
# How to clone this repository to your machine.
_Steps:_
```sh
yum install docker -y
yum install git -y
git clone https://github.com/amalbosemathew/self_signed_nginx_php_website
cd self_signed_nginx_php_website/
```

### Screenshots

Cloning the repository from Github and installating docker-compose :

![alt text](https://i.ibb.co/7N802gy/Screenshot-from-2021-06-16-19-01-39.png)


---
# Uploading the php contents to the website folder.
Here you can upload your own code in the website directory. I have used to clone my php website code stored in the github repository
```sh
cd website/
git clone https://github.com/amalbosemathew/aws-elb-site ./
```
# Creating docker container for PHP website with self-signed certicate.
Steps

```sh
docker-compose config <--------Check whether the configuration in yaml is correct.
docker-compose up -d <---------Creating the container in detach mode.(To reuse the same screen)
docker container ls -a <-------Listing all the container.

```
```sh
docker-compose down -v <--------To stop containers created using the docker-compose and to remove containers, volumes and networks.
```

### Screenshots

![alt text](https://i.ibb.co/yR7WQfb/Screenshot-from-2021-06-16-19-01-48.png)

![alt text](https://i.ibb.co/dkrLvVT/Screenshot-from-2021-06-16-19-02-38.png)

# Conclusion

The Intention of this Reposistory is to showcase the php website using Docker-compose.

<p align="center">
<a href="mailto:mathew.amalbose@gmail.com"><img src="https://img.shields.io/badge/-mathew.amalbose@gmail.com-D14836?style=flat&logo=Gmail&logoColor=white"/></a>
<a href="https://www.linkedin.com/in/amal-bose-mathew"><img src="https://img.shields.io/badge/-Linkedin-blue"/></a>
<a href="https://techbit-new.blogspot.com/"><img src="https://img.shields.io/badge/-Blogger-orange"/></a>
  

