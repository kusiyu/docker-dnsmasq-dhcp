# docker-dnsmasq-dhcp
## Introduce
Easy to build DHCP of DNSmasq images and container.
## Install docker-ce
[Install link](https://docs.docker.com/install/linux/docker-ce/ubuntu/)
## Install docker-compose
[Install link](https://docs.docker.com/compose/)
## Make docker images
`docker build . -t docker-dnsmasq`
## Deployment container
* Copy dnsmasq file to /srv

  `docker build . -t docker-dnsmasq`

* Run docker-compose.yum

  `docker-compose up -d`
  
* You can see docker container

  `docker exec -it dnsmasq bash`
