FROM adoptopenjdk/openjdk11:alpine-jre
RUN mkdir /opt/app
COPY build/libs/*.jar /opt/app/mspr-ci-application.jar
COPY docker/jdbc.sh .
ENTRYPOINT ["jdbc.sh"]
CMD ["java", "-jar", "/opt/app/mspr-ci-application.jar"]