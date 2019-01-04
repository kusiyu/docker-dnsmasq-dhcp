############################################################
# Dockerfile to build DHCP of DNSmasq container images
# Based on Ubuntu
############################################################
FROM ubuntu
MAINTAINER kuying <gubojiu@gmail.com>

ENV DEBIAN_FRONTEND noninteractive

RUN set -eux; \
	apt update; \
	apt install -y --no-install-recommends \
		dnsmasq; \

	rm -rf /etc/dnsmasq.conf \
	rm -rf /etc/dnsmasq.d \
	rm -rf /var/lib/apt/lists/* \
	rm -rf /var/lib/apt/lists/*
EXPOSE 67/udp

CMD ["/usr/sbin/dnsmasq", "-d"]

