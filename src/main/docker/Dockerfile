FROM jeanblanchard/busybox-java:8
COPY appointmentGateway-0.1.0.jar app.jar 
ENTRYPOINT ["java","-Dspring.profiles.active=docker","-jar","/app.jar"]
EXPOSE 50000-65535
