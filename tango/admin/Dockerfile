FROM tangocs/tango-admin:1.14

MAINTAINER igor.khokhriakov@hzg.de

ADD register.sh /register.sh

ENTRYPOINT /usr/local/bin/wait-for-it.sh \
                 $TANGO_HOST \
                 --timeout=30 \
                 --strict \
                 -- /register.sh
