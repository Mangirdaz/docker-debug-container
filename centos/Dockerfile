FROM centos:latest
MAINTAINER Mangirdas Judeikis Mangirdas@Judeikis.Lt
COPY bin/centos /centos
EXPOSE 8080
RUN yum install bind-utils nmap tcpdump sysstat -y ; yum clean all

CMD ["/centos"]
