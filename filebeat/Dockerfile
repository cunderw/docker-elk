ARG ELK_VERSION

# https://www.docker.elastic.co/
FROM docker.elastic.co/beats/filebeats:${ELK_VERSION}

# Add your kibana plugins setup here
# Example: RUN kibana-plugin install <name|url>
RUN filebeat modules enable nginx
# RUN filebeat setup
