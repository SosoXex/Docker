FROM    ubuntu:20.04
RUN apt update -y
RUN apt install -y default-jdk
RUN apt install -y maven
RUN apt install -y tomcat9
EXPOSE 8080
ENV CATALINA_HOME=/usr/share/tomcat9
ENV CATALINA_BASE=/var/lib/tomcat9
ENV CATALINA_TMPDIR=/tmp
#ENV JAVA_OPTS=-Djava.awt.headless=true
#RUN export PATH=$PATH:$CATALINA_HOME/bin
RUN apt-get install -y git
RUN git clone https://github.com/koddas/war-web-project.git
CMD ["/usr/share/tomcat9/bin/catalina.sh","run"]
#CMD ["cd", "war-web-project/"]
#CMD ["mvn", "package"]
#CMD ["cp","target/.war","/var/lib/tomcat9/webapps/"]





