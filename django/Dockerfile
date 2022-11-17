FROM python:3.10

ENV PYTHONUNBUFFERD 1

RUN apt-get -y update
RUN apt-get -y install vim

RUN pip install --upgrade pip

COPY ./requirements.txt /requirements.txt
RUN pip install -r /requirements.txt

COPY . /app

# runserver
CMD python manage.py runserver 0.0.0.0:8000