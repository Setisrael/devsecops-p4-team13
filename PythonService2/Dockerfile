FROM python:3.13.0a3-slim

WORKDIR /app
COPY requirements.txt /app/

RUN \
    apk add --no-cache gcc musl-dev libffi libffi-dev && \
    pip install -r requirements.txt

COPY . /app

ENTRYPOINT ["python", "app.py"]
