FROM openjdk:8-jdk-alpine
COPY /target/<nombredeapp>.jar /usr/src/service/service.jar
COPY setup.sh /
RUN chmod 777 /setup.sh
ENV LOG_LEVEL_SYSTEM=ERROR
ENV LOG_LEVEL_BUSINESS=INFO
EXPOSE 8031

CMD [ "/setup.sh" ]