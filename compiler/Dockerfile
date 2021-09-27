FROM maven:alpine
WORKDIR /app
RUN apk add git
RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git .
RUN mvn -T 1C -Dmaven.test.skip clean package
RUN ls -la ./target
