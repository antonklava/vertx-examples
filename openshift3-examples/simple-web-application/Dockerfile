
FROM java:8-jre-alpine

ENV JAVA_APP_JAR simple-web-application-3.3.0-fat.jar

EXPOSE 8080

ADD target/$JAVA_APP_JAR /app/
RUN chmod 777 /app/

WORKDIR /app/
ENTRYPOINT ["sh", "-c"]
CMD ["java -jar $JAVA_APP_JAR"]