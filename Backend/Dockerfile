FROM centos:7

LABEL Devops ="Anup_Dudhe"

RUN yum install java-11-openjdk -y
ADD https://dlcdn.apache.org/tomcat/tomcat-8/v8.5.99/bin/apache-tomcat-8.5.99.tar.gz /opt 
RUN tar -xzvf /opt/apache-tomcat-8.5.99.tar.gz -C /opt/
 

WORKDIR /opt/apache-tomcat-8.5.99/
ADD https://s3-us-west-2.amazonaws.com/studentapi-cit/mysql-connector.jar lib/mysql-connector.jar
COPY student.war webapps/student.war
COPY context.xml conf/contex.xml




EXPOSE 8080
CMD bin/catalina.sh start






