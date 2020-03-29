FROM adoptopenjdk/openjdk11:alpine-jre
RUN mkdir /opt/app
COPY build/libs/*.jar /opt/app/mspr-ci-application.jar
CMD ["java", "-jar", "/opt/app/mspr-ci-application.jar"]