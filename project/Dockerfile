FROM python:3.8-slim-bullseye

COPY ./techtrends /techtrends
WORKDIR /techtrends
RUN pip install -r requirements.txt

EXPOSE 3111

RUN python init_db.py

# command to run on container start
CMD [ "python", "app.py" ]
