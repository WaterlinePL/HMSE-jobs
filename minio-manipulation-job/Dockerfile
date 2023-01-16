FROM alpine:3.17.0

# Install minio client
RUN wget https://dl.min.io/client/mc/release/linux-amd64/mc
RUN chmod +x mc
RUN mv mc /bin/mc
RUN apk add --no-cache --upgrade bash zip

COPY init.sh .
RUN chmod +x init.sh

# Assumes folowing launch:
# sh init.sh "command1" "command2" ...
# CMD ["bash", "init.sh", "<command1>", "<command2>"]