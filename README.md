# docker-dnsmasq-dhcp
## Introduce
## Install docker-ce
## Install docker-compose
## Make docker images
`docker build . -t docker-dnsmasq`
## Deployment container
* Copy dnsmasq file to /srv
`docker build . -t docker-dnsmasq`
* Run docker-compose.yum
`docker-compose up -d`
* You can see docker container
`docker exec -it dnsmasq bash`
