# Based on Ubuntu
FROM alpine

# OpenRC manages the services, startup and shutdown of a host
RUN apk add openrc 
# ansible to remote managment
RUN apk add ansible
# openssh, ssh client, server and tools
RUN apk add openssh
RUN rc-update add sshd
RUN /etc/init.d/sshd start

# Expose ssh port
EXPOSE 22

