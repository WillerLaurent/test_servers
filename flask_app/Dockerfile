FROM python:3.9

RUN apt-get update && apt-get install -y vim
RUN apt-get install -y python-pip

WORKDIR /flask_app
COPY requirements.txt app/requirements.txt
RUN pip install --no-cache-dir -r app/requirements.txt
COPY . .
# EXPOSE 5000
# RUN nginx
# COPY start.sh ./
# CMD [ "python", "./app/main.py"]
# CMD bash start.sh

