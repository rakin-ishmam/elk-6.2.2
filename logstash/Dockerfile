FROM docker.elastic.co/logstash/logstash:7.1.1


RUN echo "removing pipeline"
RUN ls /usr/share/logstash/pipeline/
RUN rm -f /usr/share/logstash/pipeline/logstash.conf

RUN echo "removed pipeline"
RUN ls /usr/share/logstash/pipeline/

RUN echo "updating pipeline"
ADD pipeline/ /usr/share/logstash/pipeline/
RUN echo "updated pipeline"
RUN ls /usr/share/logstash/pipeline/
# ADD config/ /usr/share/logstash/config/