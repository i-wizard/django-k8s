FROM python:3.9.5-slim

COPY . /app
WORKDIR /app

RUN python -m venv /opt/venv
RUN /opt/venv/bin/pip install pip --upgrade && \
    /opt/venv/bin/pip install requirements.txt &&  \
    chmod +x entrypoint.sh

CMD [ "/app/entrypoint.sh" ]