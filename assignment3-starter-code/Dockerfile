### Docker file 
# https://docs.docker.com/get-started/02_our_app/
# https://docs.docker.com/get-started/overview/
FROM python:3.9-slim
## slim makes it smaller?
WORKDIR /usr/src/app
#WORKDIR /usr/src/app 

COPY . .

RUN pip install --no-cache-dir -r requirements.txt

EXPOSE  5000

ENV NAME World

CMD ["python", "./app.py"]

#make image 
# if no tag it will default to latest
# docker build -t image-name:tag .
# docker run image-name:tag
##############################
# pushing 
# docker login 
# docker tag image docker_account/image:tag
# docker push docker_account/image:tag