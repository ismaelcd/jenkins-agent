FROM jenkins/jenkins

## Change user to perform privileged actions
USER 0
## Install 'docker'
RUN apt update && apt install  docker -y
RUN apt install docker-compose -y
## Revert to the original non-root user
USER 1001
