FROM ubuntu

WORKDIR /wordsdocker
COPY pom.xml ./
COPY src/ ./src/

RUN apt-get update
RUN apt-get install maven openjdk-8-jdk -y

RUN mvn verify
WORKDIR /wordsdocker/target/

CMD java -Xmx8m -Xms8m -jar words.jar
EXPOSE 8080