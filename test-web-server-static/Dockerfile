FROM ubuntu:16.04
MAINTAINER Joshua Jorel Lee <joshua.jorel.lee@gmail.com>

RUN apt-get update && apt-get install -y python-pip && pip install flask
ADD app.py /opt/app.py
WORKDIR /opt
ENV FLASK_APP app.py
EXPOSE 5000
ENTRYPOINT ["python", "app.py"]