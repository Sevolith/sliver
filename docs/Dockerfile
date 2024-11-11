FROM python:3-slim


RUN apt update && apt install -y unzip

COPY www.zip /opt/

RUN unzip -o /opt/www.zip -d /opt/

EXPOSE 8000

WORKDIR /opt/out



CMD python -m http.server 8000