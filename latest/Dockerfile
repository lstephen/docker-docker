FROM ubuntu:14.04
MAINTAINER levi.stephen@gmail.com

RUN apt-get update && apt-get install -y curl

RUN curl -sSL https://get.docker.com/ubuntu/ | sh

ADD ./wrapdocker /usr/local/bin/wrapdocker
RUN chmod +x /usr/local/bin/wrapdocker

VOLUME /var/lib/docker
CMD ["wrapdocker"]
ENTRYPOINT ["wrapdocker"]

