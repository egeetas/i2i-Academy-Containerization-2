# i2i Academy Containerization Homework 2

This project demonstrates how to deploy a simple Nginx web server using Docker Compose both locally and on a Google Cloud Virtual Machine.

## Project Structure

```
.
├── docker-compose.yml
├── index.html
└── README.md
```

## Technologies Used

- Docker
- Docker Compose
- Nginx
- Google Cloud Platform (GCP)
- Ubuntu Linux

## Local Deployment

Start the container:

```bash
docker compose up -d
```

Verify that the container is running:

```bash
docker ps
```

Access the application:

```text
http://localhost:8080
```

### Screenshot - Local Docker Deployment

[INSERT LOCAL DOCKER SCREENSHOT HERE]

### Screenshot - Local Browser Access

[INSERT LOCALHOST SCREENSHOT HERE]

---

## Google Cloud VM Deployment

Clone the repository:

```bash
git clone https://github.com/egeetas/i2i-Academy-Containerization-2.git
cd i2i-Academy-Containerization-2
```

Run the container:

```bash
docker compose up -d
```

Verify the deployment:

```bash
docker ps
curl http://localhost:8080
```

### Screenshot - VM Deployment

[INSERT VM TERMINAL SCREENSHOT HERE]

### Screenshot - VM Verification

[INSERT CURL SCREENSHOT HERE]

---

## Firewall Configuration

A firewall rule was created to allow inbound TCP traffic on port 8080.

### Screenshot - Firewall Rule

[INSERT FIREWALL SCREENSHOT HERE]

---

## Public Access

The application was successfully accessed through the VM's public IP address.

Example:

```text
http://35.241.129.163:8080
```

### Screenshot - Public Access

[INSERT PUBLIC IP SCREENSHOT HERE]

---

## Result

The Nginx container was successfully deployed using Docker Compose on both a local machine and a Google Cloud VM. Access to the application was verified locally and through the VM's public IP address.
