FROM    ubuntu:16.04
RUN     apt-get update
RUN     apt-get install -y nginx
EXPOSE  80
RUN     rm -rf /var/www/html/*
VOLUME  /home/ubuntu/volune/mnt
RUN     touch /home/ubuntu/volune/mnt/1
ADD     index.html /var/www/html/
CMD     ["nginx", "-g", "daemon off;"]

