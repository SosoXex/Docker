FROM    ubuntu:20.04
RUN     apt update -y
RUN     apt-get install -y tomcat9
EXPOSE  8080
ENV CATALINA_HOME /var/lib/tomcat9
ENV PATH /usr/share/tomcat9/bin:$PATH
RUN     rm -rf /var/lib/tomcat9/webapps/ROOT/index.html
ADD     index.html /var/lib/tomcat9/webapps/ROOT/
CMD ["catalina.sh", "run"]

