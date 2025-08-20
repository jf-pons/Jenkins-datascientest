# Dockerfile to build a flask app
FROM jenkins/jenkins:lts-jdk17


USER root

COPY install_docker.sh install_docker.sh
RUN ./install_docker.sh
RUN apt install sudo

RUN apt install -y python3 python3-pip

RUN usermod -aG docker jenkins

# USER jenkins