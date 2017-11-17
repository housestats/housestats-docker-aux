FROM fedora
RUN yum -y install python3 python3-virtualenv git
RUN python3 -m virtualenv /app
RUN . /app/bin/activate; pip install git+https://github.com/larsks/neurio-export-mqtt
ENTRYPOINT ["/app/bin/neurio-export-mqtt"]
