FROM fedora
RUN yum -y install python3 python3-virtualenv git
RUN python3 -m virtualenv /app
RUN . /app/bin/activate; pip install git+https://github.com/larsks/openweather-mqtt-export
ENTRYPOINT ["/app/bin/owm-export-mqtt"]
