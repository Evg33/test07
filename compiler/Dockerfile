FROM ubuntu:20.04
RUN apt-get update && apt-get install -y default-jdk maven git
RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git /tmp/bf/
RUN mvn -T 1C -Dmaven.test.skip package --file /tmp/bf/

