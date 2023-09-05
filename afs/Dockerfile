FROM common_scripts

RUN apt-get -qq -y update && \
  DEBIAN_FRONTEND=noninteractive apt-get install -y vim krb5-user \
    openafs-client openafs-modules-dkms openafs-krb5 openafs-fileserver openafs-dbserver && \
  apt-get clean

COPY init-script.sh /tmp/
CMD /tmp/init-script.sh
