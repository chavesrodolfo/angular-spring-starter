FROM openjdk:8

VOLUME /tmp
RUN mkdir /app
WORKDIR /app
COPY ./target/angular-spring-starter.jar ./angular-spring-starter.jar
RUN bash -c 'touch angular-spring-starter.jar'

CMD ["java", "-Djava.security.egd=file:/dev/./urandom", "-jar", "angular-spring-starter.jar"]