FROM docker.elastic.co/kibana/kibana:5.5.1

ENV ELASTICSEARCH_URL=http://jhipster-elasticsearch:9200
COPY kibana.yml /usr/share/kibana/config/kibana.yml
RUN ./bin/kibana-plugin install https://github.com/sivasamyk/logtrail/releases/download/v0.1.18/logtrail-5.5.1-0.1.18.zip
RUN ./bin/kibana-plugin install https://github.com/sirensolutions/sentinl/releases/download/tag-5.5/sentinl-v5.5.1.zip
RUN ./bin/kibana-plugin install https://github.com/PierreBesson/kbn_c3js_vis/releases/download/V5.5.1/c3_charts-v5.5.1.zip
COPY logtrail.json /usr/share/kibana/plugins/logtrail/logtrail.json