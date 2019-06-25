FROM python:2.7
RUN pip install elastalert
WORKDIR /home/elastalert
COPY config.yaml /home/elastalert/config.yaml
COPY error.yaml /home/elastalert/error.yaml
ENTRYPOINT ["elastalert", "--verbose", "--rule", "error.yaml"]