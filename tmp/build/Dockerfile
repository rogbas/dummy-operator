FROM alpine:3.6

RUN adduser -D dummy-operator
USER dummy-operator

ADD tmp/_output/bin/dummy-operator /usr/local/bin/dummy-operator
