ARG ELASTIC_VERSION

# https://www.docker.elastic.co/
FROM docker.elastic.co/logstash/logstash:${ELASTIC_VERSION}

# Create data dir
RUN mkdir /var/logstash_data

# Load pipeline
ENTRYPOINT logstash -f pipeline/logstash_world_countries.conf

# Add your logstash plugins setup here
# Example: RUN logstash-plugin install logstash-filter-json
