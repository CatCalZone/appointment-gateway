FROM jeanblanchard/busybox-java:8
VOLUME /tmp
ADD build/libs/appointmentGateway-0.1.0.jar 
RUN bash -c 'touch /appointmentGateway-0.1.0.jar'
ENTRYPOINT ["java","-Dspring.profiles.active=docker -Djava.security.egd=file:/dev/./urandom","-jar","/appointmentGateway-0.1.0.jar"]
EXPOSE 50000-65535
