FROM php:latest

RUN mkdir /build
WORKDIR /build

RUN go get git@github.com:Georgeclark04/dockertest.git
RUN cd /build && git clone git@github.com:Georgeclark04/dockertest.git

RUN cd/build/dockertest/php && go build

EXPOSE 8080

ENTRYPOINT [ "/build/dockertest/php" ]



