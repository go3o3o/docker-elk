ARG ELK_VERSION

# https://www.docker.elastic.co/
FROM docker.elastic.co/elasticsearch/elasticsearch:${ELK_VERSION}

# Add your elasticsearch plugins setup here

COPY config/medi_dictionary.txt config/medi_dictionary.txt

# 한글 형태소 분석
RUN elasticsearch-plugin install analysis-nori
# 오타 교정
RUN elasticsearch-plugin install analysis-icu