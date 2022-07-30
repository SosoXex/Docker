FROM    ubuntu:20.04
RUN apt update -y
RUN apt install -y default-jdk
RUN apt install -y maven
RUN apt install -y tomcat9
EXPOSE 8080
RUN export CATALINA_HOME=/usr/share/tomcat9
RUN export CATALINA_BASE=/var/lib/tomcat9
RUN export CATALINA_TMPDIR=/tmp
RUN JAVA_OPTS=-Djava.awt.headless=true
RUN apt-get install -y git
RUN git clone https://github.com/koddas/war-web-project.git
CMD ["/usr/share/tomcat9/startup.sh", "run"]
#CMD ["cd", "war-web-project/"]
#CMD ["mvn", "package"]
#CMD ["cp","target/.war","/var/lib/tomcat9/webapps/"]





