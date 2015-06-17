FROM jeanblanchard/busybox-java:8
VOLUME /tmp
ADD build/libs/appointmentGateway-0.1.0.jar app.jar 
RUN bash -c 'touch /app.jar'
ENTRYPOINT ["java","-Dspring.profiles.active=docker -Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]
EXPOSE 50000-65535
