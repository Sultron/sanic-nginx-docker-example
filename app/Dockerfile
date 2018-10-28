FROM python:3.7.0

EXPOSE 5000

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

RUN apt-get install libssl-dev libffi-dev

COPY requirements.txt /usr/src/app/
RUN pip install --no-cache-dir -r requirements.txt
COPY . /usr/src/app
