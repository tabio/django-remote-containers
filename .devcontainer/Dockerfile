FROM python:3.10.7-slim

RUN apt-get update && apt-get install -y --no-install-recommends \
     build-essential default-libmysqlclient-dev default-mysql-client

ADD requirements.txt .
RUN pip install --no-cache-dir --user -r requirements.txt
ENV PATH=$PATH:/root/.local/bin

ENV PYTHONUNBUFFERED 1
ENV PYTHONDONTWRITEBYTECODE 1

