FROM python:3.9-slim
WORKDIR /app
COPY requirements.txt ./
RUN apt-get update && apt-get install -y python3-pip && pip3 install --no-cache-dir -r requirements.txt
COPY . .
CMD ["gunicorn", "--bind", "0.0.0.0:9000", "kittygram_backend.wsgi"]