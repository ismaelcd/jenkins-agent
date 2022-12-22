FROM jenkins/inbound-agent

## Cambiamos a usuario con poermisos
USER 0

## Install packages
RUN apt update && apt install iputils-ping net-tools docker docker-compose -y
CMD ["ping", "www.google.es"]
RUN gpasswd -a jenkins docker
RUN usermod -aG docker jenkins

USER 1000
