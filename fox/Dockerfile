FROM ubuntu:14.04

RUN apt update && \
	apt upgrade -y && \
	apt install -y gcc valgrind make git && \
	mkdir /git

WORKDIR /git
