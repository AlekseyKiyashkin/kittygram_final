FROM python:3.9-slim
WORKDIR /app
COPY requirements.txt .
RUN apt-get update && apt-get install -y python3-pip && pip3 install --no-cache-dir -r requirements.txt
COPY . .
RUN chmod u+x bootstrap.sh
CMD ["./bootstrap.sh"]
EXPOSE 9000