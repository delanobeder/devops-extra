FROM tomcat:7.0-jdk8

LABEL maintainer="auri@ufscar.br, g4briel.4lves@gmail.com"

ADD catalina.sh /usr/local/tomcat/bin/
ADD .keystore /usr/local/tomcat/conf/
ADD server.xml /usr/local/tomcat/conf/
ADD context.xml /usr/local/tomcat/conf/
ADD sample.war /usr/local/tomcat/webapps/
ADD devopsnapratica.war /usr/local/tomcat/webapps/

EXPOSE 8080
EXPOSE 8443

RUN chmod a+x /usr/local/tomcat/bin/catalina.sh

CMD ["catalina.sh", "run"]