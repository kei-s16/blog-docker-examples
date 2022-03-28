ARG TAG="3.10.4-bullseye"

FROM python:$TAG as build
WORKDIR /usr/src/app
COPY ./src/requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt

FROM build as app
COPY ./src .
CMD ["python", "main.py"]
