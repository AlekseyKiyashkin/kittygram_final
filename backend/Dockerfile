FROM python:3.9-alpine
WORKDIR /app 
COPY requirements.txt ./ 
RUN pip3 install -r requirements.txt --no-cache-dir 
COPY . . 
CMD ["gunicorn", "--bind", "0.0.0.0:9000", "kittygram_backend.wsgi"] 