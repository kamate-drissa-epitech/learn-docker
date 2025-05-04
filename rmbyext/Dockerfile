FROM python:3-alpine

WORKDIR /zone

RUN apk add --no-cache git && \
    git clone https://github.com/fhsinchy/rmbyext.git && \
    cp rmbyext/rmbyext.py /usr/local/bin/rmbyext && \
    chmod +x /usr/local/bin/rmbyext && \
    apk del git

ENTRYPOINT [ "rmbyext" ]
    