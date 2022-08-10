FROM python:3.7.8rc1

COPY . /app
WORKDIR /app

RUN python3 -m venv /opt/venv

RUN pip install pip --upgrade && \
    /opt/venv/bin/pip install -r requirements.text && \
    chmod +x entrypoint.sh

CMD [ "/app/entrypoint.sh" ]