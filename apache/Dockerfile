FROM centos:centos6
MAINTAINER jacksyen <hyqiu.syen@gmail.com>
RUN yum -y install httpd 
RUN yum -y install httpd-devel
RUN sed -i 's/Listen 80/Listen 8080/g' /etc/httpd/conf/httpd.conf
EXPOSE 8080
ENTRYPOINT ["/usr/sbin/httpd"] 
CMD ["-D", "FOREGROUND"]
