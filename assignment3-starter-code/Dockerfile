### Docker file 
# https://docs.docker.com/get-started/02_our_app/
# https://docs.docker.com/get-started/overview/
From python:3.9-slim
## slim makes it smaller?
WORKDIR usr/src/app

COPY . .

RUN pip install --no-cache-dir -r requirements.txt

EXPOSE  5000

ENV NAME World

CMD ["python", "./app.py"]

#make image 
# docker build -t image-name .