FROM tomcat:8.0
RUN apt-get update && apt-get install wget
##COPY index.html /usr/local/tomcat/webapps/ROOT/index.html
ADD https://tomcat.apache.org/tomcat-5.5-doc/appdev/sample/sample.war /usr/local/tomcat/webapps/sample.war
USER root
WORKDIR /usr/local/tomcat
CMD ["catalina.sh", "run"]
EXPOSE 8080
