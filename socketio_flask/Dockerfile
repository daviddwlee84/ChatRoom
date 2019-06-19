FROM python:alpine

# for cython & gcc support (e.g. greenlet)
# https://github.com/docker-library/python/issues/312
# https://github.com/docker-library/python/issues/318
RUN apk add gcc musl-dev python3-dev
RUN pip3 install cython

LABEL Name=chatroom Version=0.0.1
EXPOSE 5000

WORKDIR /app
ADD . /app

RUN python3 -m pip install -r requirements.txt
CMD ["python3", "-m", "chatroom"]
