FROM fluent/fluentd:v1.5-1

USER root

RUN apk add tzdata && \
    gem install fluent-plugin-s3 && \
    cp /usr/share/zoneinfo/Asia/Tokyo /etc/localtime

COPY fluent.conf /fluentd/etc/

USER fluent