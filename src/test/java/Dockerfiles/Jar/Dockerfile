FROM openjdk:8-jre-alpine
RUN java -version
# copy application WAR (with libraries inside)
COPY /npweb-0.0.1-SNAPSHOT.jar /npweb-app.jar
# specify default command
CMD ["/usr/bin/java", "-jar", "/npweb-app.jar"]