FROM ubuntu:focal

RUN apt-get update && \
    apt-get --no-install-recommends install mycli=1.20.1-4 iputils-ping=3:20190709-3 -y && \
    apt-get clean && rm -rf /var/lib/apt/lists/*

CMD ["sleep", "infinity"] # Keep the container running
