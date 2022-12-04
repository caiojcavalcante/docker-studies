FROM python:3.10

ENV PYTHONBUFFERED=1

WORKDIR /code

RUN pip install --upgrade pip

COPY requirements.txt .

RUN pip install -r requirements.txt

COPY . .

ARG BUILD_PORT=8000

EXPOSE $BUILD_PORT

CMD ["python","manage.py","runserver"]