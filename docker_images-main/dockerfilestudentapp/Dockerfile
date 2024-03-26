
FROM centos:7 
LABEL dev="anup"

ADD https://dlcdn.apache.org/tomcat/tomcat-8/v8.5.98/bin/apache-tomcat-8.5.98.zip /opt
RUN unzip apache-tomcat-8.5.98.zip  /opt
RUN yum install java-11-openjdk -y


USER root

WORKDIR /opt/apache-tomcat-8.5.98/
ADD https://s3-us-west-2.amazonaws.com/studentapi-cit/student.war  /opt/apache-tomcat-8.5.98/webapps/
 
CMD bin/apache-tomcat-8.5.98/catalina.sh run 

EXPOSE 8080


