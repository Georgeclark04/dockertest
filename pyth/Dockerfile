FROM python:latest

RUN mkdir /build 
WORKDIR /build

RUN cd /build && git clone git@github.com:Georgeclark04/dockertest.git

RUN cd /build/dockertest/pyth/ && go build

EXPOSE 8080

ENTRYPOINT [ "/build/dockertest/pyth/app" ]