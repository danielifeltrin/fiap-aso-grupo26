FROM openjdk:latest
MAINTAINER Grupo 26  <dpfeltrin@gmail.com>
LABEL description="Dockerfile para SOLUTION SPRINT - CONTAINERIZATION STRATEGY"
ENV HW_HOME=/opt/hello-world
ADD HelloWorld.class $HW_HOME/
WORKDIR $HW_HOME
ENTRYPOINT ["java", "HelloWorld"]
