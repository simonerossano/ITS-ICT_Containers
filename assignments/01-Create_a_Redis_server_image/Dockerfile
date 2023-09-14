FROM ubuntu:latest
LABEL MANTAINER="Simone Rossano"
RUN apt update && apt install -y redis-server
COPY ./redis.conf /etc/redis
EXPOSE 6380/tcp
USER redis

ENTRYPOINT [ "redis-server", "/etc/redis/redis.conf" ]

