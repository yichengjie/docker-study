FROM elasticsearch:7.6.2
MAINTAINER yicj
COPY elasticsearch-analysis-ik-7.6.2.zip elasticsearch-analysis-ik-7.6.2.zip
WORKDIR /usr/share/elasticsearch/bin
RUN ./elasticsearch-plugin install -b file:////usr/share/elasticsearch/elasticsearch-analysis-ik-7.6.2.zip