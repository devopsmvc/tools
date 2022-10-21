FROM ubuntu:16.04
LABEL maintainer='Mahesh Varma'
RUN apt-get update -y
RUN apt-get install apache2 -y
RUN apt-get install wget -y
RUN apt-get install unzip -y
RUN apt-get install git -y
WORKDIR /tmp
RUN wget https://github.com/mditsolutions1/html/archive/main.zip
RUN unzip main.zip
RUN cp -r html-main/* /var/www/html/
EXPOSE 80
CMD ["apachectl", "-D", "FOREGROUND"]