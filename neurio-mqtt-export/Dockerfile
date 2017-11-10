FROM fedora
RUN yum -y install python3 python3-virtualenv git
RUN python3 -m virtualenv /neurio
RUN . /neurio/bin/activate; pip install git+https://github.com/larsks/neurio-export-mqtt
ENTRYPOINT ["/neurio/bin/neurio-export-mqtt"]
