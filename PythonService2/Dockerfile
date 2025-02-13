FROM python:3.14.0a1-slim-bookworm

WORKDIR /app
COPY requirements.txt /app/

RUN \
    apk add --no-cache gcc musl-dev libffi libffi-dev && \
    pip install -r requirements.txt

COPY . /app

ENTRYPOINT ["python", "app.py"]
