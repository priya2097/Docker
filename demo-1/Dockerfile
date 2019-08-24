FROM tomcat

EXPOSE 8080

#RUN mvn clean package

COPY .  /usr/local/tomcat/

WORKDIR /usr/local/tomcat/

#ADD target/spring_boot_demo-0.0.1-SNAPSHOT.war  /usr/local/tomcat/webapps/
ADD  target/spring.war /usr/local/tomcat/webapps/spring.war

#WORKDIR /usr/local/tomcat

COPY tomcat-users.xml /usr/local/tomcat/conf/tomcat-users.xml
COPY context.xml /usr/local/tomcat/webapps/manager/META-INF/context.xml


