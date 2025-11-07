FROM --platform=linux/amd64 tomcat:8.5-jre8-temurin
COPY drop/*.war /usr/local/tomcat/webapps/ROOT.war

COPY drop/* /usr/local/tomcat/webapps/

EXPOSE 8080

CMD ["/usr/local/tomcat/bin/catalina.sh", "run"]
