FROM python:3

RUN apt-get update -y
RUN pip3 install flask
RUN useradd -ms /bin/bash backend
WORKDIR /home/backend

COPY /app /home/backend/app

WORKDIR /home/backend/app

RUN chmod 777 ./create_student.sh

EXPOSE 5000
ENTRYPOINT [ "bash", "/home/backend/app/create_student.sh" ]
CMD [ "python", "/home/backend/app/web.py" ]