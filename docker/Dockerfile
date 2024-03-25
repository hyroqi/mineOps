#Base image
FROM openjdk:17.0.1-jdk-oraclelinux8

#create and go to directory
RUN mkdir /minecraft
WORKDIR /minecraft

#copy files to new directory
COPY eula.txt .
COPY server.jar .

#running the server
CMD ["java", "-jar", "server.jar"]