# Dockerfile for book_catalog microservice


FROM python:3.10-slim

WORKDIR /app

COPY book_catalog/requirements.txt /app/requirements.txt

RUN pip install --no-cache-dir -r requirements.txt

COPY book_catalog /app

EXPOSE 8000

CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]
