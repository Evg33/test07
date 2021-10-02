#img size 106.5 MB

FROM tomcat:alpine AS web

RUN mkdir /shared
RUN ls -la /shared
RUN ls -la /usr/local/tomcat/webapps/

ADD starter.sh /starter.sh
CMD ["/starter.sh"]
