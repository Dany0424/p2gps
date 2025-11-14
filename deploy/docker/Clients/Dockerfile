FROM --platform=linux/amd64 tomcat:8.5-jre8-temurin
COPY drop/*.war /usr/local/tomcat/webapps/ROOT.war

COPY drop/* /usr/local/tomcat/webapps/

EXPOSE 8082

ENTRYPOINT ["/bin/sh", "-c", "P=8082; sed \"s/8080/$P/g\" < conf/server.xml > /tmp/srv.xml && catalina.sh run -config /tmp/srv.xml"]
