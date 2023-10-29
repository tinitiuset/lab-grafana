FROM httpd:2.4-alpine

RUN apk add -U unzip && rm -rf /var/cache/apk/*

COPY ./webHelpLAB-GRAFANA2-all.zip /usr/local/apache2/htdocs/
RUN unzip /usr/local/apache2/htdocs/webHelpLAB-GRAFANA2-all.zip -d /usr/local/apache2/htdocs/
RUN rm /usr/local/apache2/htdocs/webHelpLAB-GRAFANA2-all.zip