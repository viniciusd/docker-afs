FROM debian:bookworm

COPY configureAFSClient.sh configureKerberosClient.sh /tmp/

RUN apt-get update && \
    apt-get install -y python3-launchpadlib software-properties-common && \ 
    add-apt-repository ppa:openafs/stable
