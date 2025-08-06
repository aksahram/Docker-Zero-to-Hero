FROM python:3.12-slim

WORKDIR /app

COPY requirements.txt /app
COPY devops /app

RUN pip install --upgrade pip && \
    pip install -r requirements.txt

ENTRYPOINT ["python3"]
CMD ["manage.py", "runserver", "0.0.0.0:8000"]
