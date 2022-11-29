FROM python:3.8

LABEL maintainer="Chijioke Eze"

COPY . /app

WORKDIR /app

# install dependencies
RUN pip install -r requirements.txt

# command to initialize the database
RUN python init_db.py

# command to execute on container start
CMD [ "python", "app.py" ]

EXPOSE 3111