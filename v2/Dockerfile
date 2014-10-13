FROM google/debian:wheezy

RUN apt-get update
RUN apt-get install -y python

RUN mkdir /web
WORKDIR /web
RUN echo Hello World > index.html

CMD ["python", "-m", "SimpleHTTPServer"]
