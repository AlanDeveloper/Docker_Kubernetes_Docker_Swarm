FROM python:3

RUN apt-get update -y
RUN apt-get install -y python3-pip
RUN apt-get install -y python3-dev

WORKDIR /app

RUN pip install Flask
RUN pip install requests

COPY . .

EXPOSE 5000

CMD ["python3", "./app.py"]