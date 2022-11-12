FROM python:3.10

ENV PYTHONUNBUFFERED 1

RUN apt-get -y update
RUN apt-get -y install vim

RUN mkdir /srv/docker-ELKsetting
ADD . /srv/docker-ELKsetting

WORKDIR /srv/docker-ELKsetting

RUN pip install --upgrade pip
RUN pip install -r requirements.txt
