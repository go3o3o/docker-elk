ARG ELK_VERSION

# https://www.docker.elastic.co/
FROM docker.elastic.co/logstash/logstash:${ELK_VERSION}

USER root

RUN mkdir /usr/share/logstash-mongodb
RUN mkdir /usr/share/logstash-mongodb/products
RUN mkdir /usr/share/logstash-mongodb/productCategories

RUN chown -R root /usr/share/logstash

# Add your logstash plugins setup here
# Example: RUN logstash-plugin install logstash-filter-json
# RUN logstash-plugin install logstash-input-mongodb
# RUN logstash-plugin install logstash-output-mongodb