ARG TAG="3.10.4-bullseye"

FROM python:$TAG
WORKDIR /usr/src/app

COPY ./src .
RUN pip install --no-cache-dir -r requirements.txt
CMD ["python", "main.py"]
