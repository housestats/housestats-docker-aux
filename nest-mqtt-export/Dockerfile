FROM fedora
RUN yum -y install python3 python3-virtualenv git
RUN python3 -m virtualenv /nest
RUN . /nest/bin/activate; pip install git+https://github.com/larsks/nest-mqtt-export
ENTRYPOINT ["/nest/bin/nest-export-mqtt"]
