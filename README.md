# Docker image for DNSmasq DHCP server
## Introduce
This Docker image is suitable for running a DHCP server for your docker host network. It uses DNSmasq DHCP server which is bundled with the latest Ubuntu 18.04 LTS distribution.
Easy to build DHCP of DNSmasq image and container.
## Install docker-ce
Install docker-ce with the instructions on <https://docs.docker.com/install/linux/docker-ce/ubuntu/>
## Install docker-compose
Install ocker-compose with the instructions on <https://docs.docker.com/compose/)>
## Build docker images
[![](https://img.shields.io/docker/automated/:user/:repo.svg)](https://cloud.docker.com/repository/docker/kusiyu/dnsmasq-dhcp/tags)

`docker build . -t docker-dnsmasq`
## Deployment container
* Copy dnsmasq files to /srv

  `cp -r dnsmasq.d dnsmasq.conf /srv`

* Run docker-compose.yum

  `docker-compose up -d`
  
* You can see docker container

  `docker exec -it dnsmasq bash`
