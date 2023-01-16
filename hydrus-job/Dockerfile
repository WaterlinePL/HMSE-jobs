FROM ubuntu:22.04

RUN apt update
RUN apt upgrade -y
RUN apt install gfortran -y

RUN echo "/workspace" >> LEVEL_01.DIR
COPY hydrus hydrus
RUN chmod +x hydrus

 CMD ["./hydrus"]
