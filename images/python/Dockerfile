FROM python:3.11-alpine

RUN adduser --home /sandbox --disabled-password sandbox

COPY requirements.txt /tmp
RUN pip install --no-cache-dir -r /tmp/requirements.txt && rm -f /tmp/requirements.txt

USER sandbox
WORKDIR /sandbox

ENV PYTHONDONTWRITEBYTECODE=1
ENV PYTHONUNBUFFERED=1
