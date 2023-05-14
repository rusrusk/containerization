FROM ubuntu:20.04

WORKDIR /usr/src/app

RUN apt-get update && apt-get install -y curl

COPY test.sh .

RUN chmod +x test.sh

ENTRYPOINT ["./test.sh"]



# FROM ubuntu:18.04

# WORKDIR /mydir

# RUN apt-get update && apt-get -y install curl python
# RUN curl -L https://yt-dl.org/downloads/latest/youtube-dl -o /usr/local/bin/youtube-dl
# RUN chmod a+rx /usr/local/bin/youtube-dl

# ENV LC_ALL=C.UTF-8

# ENTRYPOINT ["/usr/local/bin/youtube-dl"]