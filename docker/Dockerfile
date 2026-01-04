FROM eclipse-temurin:17-jre-alpine

RUN addgroup -S app && adduser -S app -G app
USER app

WORKDIR /app
COPY target/hello-1.0.0.jar app.jar

EXPOSE 8081
ENTRYPOINT ["java","-jar","/app/app.jar"]
