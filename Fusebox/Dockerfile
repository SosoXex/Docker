FROM    ubuntu:20.04
RUN     apt update -y
RUN     apt-get install -y nginx
EXPOSE  8081
RUN     rm -rf /var/www/html/*
ADD     index.html /var/www/html/
CMD     ["nginx", "-g", "daemon off;"]

