# docker-dnsmasq-dhcp
## Introduce
Easy to build DHCP of DNSmasq image and container.
## Install docker-ce
[Install link](https://docs.docker.com/install/linux/docker-ce/ubuntu/)
## Install docker-compose
[Install link](https://docs.docker.com/compose/)
## Build docker images
[![](https://img.shields.io/docker/automated/:user/:repo.svg)](https://cloud.docker.com/repository/docker/kusiyu/dnsmasq-dhcp/tags)
`docker build . -t docker-dnsmasq`
## Deployment container
* Copy dnsmasq files to /srv

  cp -r dnsmasq.d dnsmasq.conf /srv

* Run docker-compose.yum

  `docker-compose up -d`
  
* You can see docker container

  `docker exec -it dnsmasq bash`
