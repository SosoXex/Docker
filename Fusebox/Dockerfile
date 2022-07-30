FROM    tomcat:9
RUN apt-get update -y
RUN apt-get install -y default-jdk
RUN apt-get install -y maven
EXPOSE 8080
RUN apt-get install -y git
CMD ["git", "clone", "https://github.com/koddas/war-web-project.git"]
CMD ["catalina.sh", "run"]




