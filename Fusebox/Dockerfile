FROM    tomcat:9
RUN apt-get update -y
RUN apt-get install -y default-jdk
RUN apt-get install -y maven
EXPOSE 8080
CMD ["/opt/tomcat/bin/catalina.sh", "run"]




