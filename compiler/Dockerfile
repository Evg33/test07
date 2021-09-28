#img size 147.2 MB
FROM maven:alpine
WORKDIR /app
RUN apk --no-cache add git
RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git .
RUN mvn -T 1C -Dmaven.test.skip package
