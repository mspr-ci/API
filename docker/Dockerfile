FROM adoptopenjdk/openjdk11:alpine-jre
RUN mkdir /opt/app
COPY build/libs/*.jar /opt/app/mspr-ci-application.jar
CMD ["java", "-agentlib:jdwp=transport=dt_socket,server=y,suspend=n,address=8341", "-jar", "/opt/app/mspr-ci-application.jar"]