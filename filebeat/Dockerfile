ARG ELK_VERSION

# https://www.docker.elastic.co/
FROM docker.elastic.co/beats/filebeat:${ELK_VERSION}

USER root
# Add your kibana plugins setup here
# Example: RUN kibana-plugin install <name|url>
# RUN mkdir /usr/share/filebeat/dockerlogsl
# RUN chown -R root /usr/share/filebeat/
RUN chmod -R go-w /usr/share/filebeat/
RUN filebeat setup --pipelines --modules nginx,system ---dashboards
