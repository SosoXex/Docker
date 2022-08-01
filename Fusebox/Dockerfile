FROM    ubuntu:18.04
RUN apt update -y
ADD requirements.txt /tmp/
RUN apt-get install -y python-all python-pip
WORKDIR /tmp
RUN pip install -qr requirements.txt
ADD app.py /opt/webapp/
EXPOSE 5000
WORKDIR /opt/webapp
CMD ["python","app.py"]





