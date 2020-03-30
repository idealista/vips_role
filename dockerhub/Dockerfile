FROM debian:buster-20200224-slim
LABEL maintainer="idealista <labs@idealista.com>"

RUN rm -rf /var/lib/apt/lists/* \
    && apt-get update \
    && apt-get -y install python3-minimal \
    && apt-get autoremove -y \
    && apt-get clean

CMD ["sleep", "infinity"]