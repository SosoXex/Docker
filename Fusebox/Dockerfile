FROM    ubuntu:20.04
RUN     apt update -y
RUN     apt-get install -y tomcat9
EXPOSE  8080
RUN     rm -rf /var/lib/tomcat9/webapps/ROOT/index.html
ADD     index.html /var/lib/tomcat9/webapps/ROOT/
CMD ["bash"]

