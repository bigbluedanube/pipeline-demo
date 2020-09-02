#This is a comment.
FROM tomcat:8-jre8-alpine
#Next line cleans the webapp folder.
RUN rm -rf /usr/local/tomcat/webapps/*
#Next line copies the artifact (the .war file) from the directory that holds the Dockerfile and places it in the tomcat webapps folder.
COPY HelloServlets.war /usr/local/tomcat/webapps/HelloServlets.war
#Next line: When the container "spins up", CMD is a command that tells Tomcat to run catalina.sh with that .war file in the webapps folder. 
CMD ["catalina.sh", "run"]