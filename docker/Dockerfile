FROM centos:latest
MAINTAINER adi adi3399@gmail.com
RUN yum install httpd -y
RUN echo "ServerName localhost" >> /etc/httpd/conf/httpd.conf
RUN sed -i 's/Listen 80/Listen 8080/g' /etc/httpd/conf/httpd.conf
COPY index.html /var/www/html/
CMD ["/usr/sbin/httpd", "-D", "FOREGROUND"]
EXPOSE 8080
