✅ Task 1: Docker & Containerization
Docker enables lightweight, portable application packaging.
Virtualization vs Containerization: VMs run entire OS, containers share host kernel → faster, smaller, ideal for CI/CD & microservices.

✅ Task 2: Sample Flask App + Dockerfile
📄 app.py

from flask import Flask

app = Flask(**name**)

@app.route("/")

def hello():

return "Hello from Docker!"

if **name** == "**main**":

app.run(host="0.0.0.0", port=80)

📄 requirements.txt

nginx
flask

🐳 Dockerfile (Multi-stage build)

Dockerfile

FROM python:3.10-slim as builder

WORKDIR /app

COPY requirements.txt .

RUN pip install --user -r requirements.txt

FROM python:3.10-slim

WORKDIR /app

COPY --from=builder /root/.local /root/.local

COPY app.py .

ENV PATH=/root/.local/bin:$PATH

EXPOSE 80

CMD ["python", "app.py"]

✅ Task 3: Key Docker Concepts

Image: Blueprint of a container.

Container: Running instance.

Volume: Persistent storage.

Network: Enables container communication.

Dockerfile: Instructions to build image.

✅ Task 4: Multi-Stage Builds

Reduces image size significantly.

Clean separation of build/runtime.

Command:

docker build -t suyash700/sample-app:latest .

✅ Task 5: Docker Hub

docker tag suyash700/sample-app:latest suyash700/sample-app:v1.0

docker push suyash700/sample-app:v1.0

✅ Task 6: Docker Volumes

docker volume create my_volume

docker run -d -v my_volume:/app/data suyash700/sample-app:v1.0

✅ Task 7: Docker Networking

docker network create my_network

docker run -d --name app --network my_network suyash700/sample-app:v1.0

docker run -d --name db --network my_network -e MYSQL_ROOT_PASSWORD=root mysql:latest

✅ Task 8: Docker Compose

📄 docker-compose.yml

version: '3.8'

services:

web:

build: .

ports: [ "8080:80" ]

volumes: [ "my_volume:/app/data" ]

networks: [ "my_network" ]

db:

image: mysql

environment:

MYSQL_ROOT_PASSWORD: root

networks: [ "my_network" ]

volumes:

my_volume:

networks:

my_network:


docker-compose up -d

docker-compose down

✅ Task 9: Docker Scout

docker scout cves suyash700/sample-app:v1.0 > scout_report.txt

📝 Lists CVEs, severity, and remediation tips.

✅ Task 10: Reflection

Docker simplifies development, testing, and deployment across environments.

Key learnings: image optimization, security scanning, networking, and orchestration.
