FROM alpine:3.8

ENV OPERATOR=/usr/local/bin/operator-v0.5 \
    USER_UID=1001 \
    USER_NAME=operator-v0.5

# install operator binary
COPY build/_output/bin/operator-v0.5 ${OPERATOR}

COPY build/bin /usr/local/bin
RUN  /usr/local/bin/user_setup

ENTRYPOINT ["/usr/local/bin/entrypoint"]

USER ${USER_UID}
