FROM common_scripts

RUN apt-get -qq -y update && \
  DEBIAN_FRONTEND=noninteractive apt-get install -y vim krb5-user \
    openafs-client openafs-krb5 openafs-modules-dkms && \
  apt-get clean

COPY init-script.sh /tmp/
CMD /tmp/init-script.sh
