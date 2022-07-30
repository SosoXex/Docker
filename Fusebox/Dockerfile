FROM ubuntu:20.04
RUN apt update -y
RUN apt install -y default-jdk
RUN apt install -y git
RUN apt install -y maven
RUN apt install -y tomcat9
COPY git.link $HOME
CMD cd $HOME
CMD git clone << cat $HOME/git.link
EXPOSE 8080


