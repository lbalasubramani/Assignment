FROM python:3.9.7

COPY requirements.txt .

RUN pip -V

RUN python -m pip install -r requirements.txt


COPY . /app

WORKDIR /app

RUN python db.py

EXPOSE 80

CMD ["python", "runserver.py"]
