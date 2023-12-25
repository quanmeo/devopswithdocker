# Start from the ubuntu image
FROM ubuntu:20.04

WORKDIR /usr/src/app

COPY ask_website.sh .

RUN apt update && apt install -y curl

CMD ./ask_website.sh
