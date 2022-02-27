FROM python:3.9-slim-buster

WORKDIR /app

COPY requirements.txt .

RUN python -m pip install -r requirements.txt

COPY . /app

RUN python db.py

EXPOSE 5000

CMD [ "python", "-m", "flask", "run", "--host=0.0.0.0" ]
