#img size 147.2 MB

FROM maven:alpine AS buildapp

#RUN apk --no-cache upgrade
RUN apk --no-cache add git

RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git /opt/bf && \
  cd /opt/bf && \
  mvn -T 1C -Dmaven.test.skip package && \
  mkdir /app /shared && \
  cp target/hello-1.0.war /shared/hello-1.0.war && \
  /bin/rm -rf /opt/bf

RUN ls -la /shared
