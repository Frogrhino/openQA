FROM opensuse/leap:15.1
LABEL maintainer Jan Sedlak <jsedlak@redhat.com>, Josef Skladanka <jskladan@redhat.com>, wnereiz <wnereiz@eienteiland.org>, Sergio Lindo Mansilla <slindomansilla@suse.com>
LABEL version="0.3"

RUN zypper --non-interactive in ca-certificates-mozilla git wget

ADD data.template /data
ADD scripts /scripts
RUN chmod -R 777 /data /scripts
VOLUME ["/data"]

CMD /usr/bin/tail -f /dev/null
