FROM python:3.6-alpine

WORKDIR ./

RUN apk update
COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt

COPY ./ ./app
WORKDIR ./app

EXPOSE 8000
