FROM frolvlad/alpine-oraclejdk8:slim
VOLUME /tmp
ADD ws-service-discovery-0.0.1-SNAPSHOT.jar app.jar
RUN sh -c 'touch /app.jar'
EXPOSE 1111:1111
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]
