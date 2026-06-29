# i2i Academy Containerization Homework 2

This project demonstrates how to deploy a simple Nginx web server using Docker Compose both locally and on a Google Cloud Virtual Machine.

## Project Structure

```text
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

---

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

<img width="1161" height="408" alt="Ekran Resmi 2026-06-29 14 43 36" src="https://github.com/user-attachments/assets/70e5078a-587e-4523-bb07-9ce40ab062ae" />


### Screenshot - Local Browser Access

<img width="1512" height="982" alt="Ekran Resmi 2026-06-29 14 44 26" src="https://github.com/user-attachments/assets/b2afe2d9-e53d-4bd2-9c50-ea9de06ee06f" />


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
curl http://35.241.129.163:8080
```

### Screenshot - VM Deployment

<img width="1512" height="704" alt="Ekran Resmi 2026-06-29 15 29 35" src="https://github.com/user-attachments/assets/c542fdc7-372c-4997-8178-8c747dd5759a" />


### Screenshot - VM Verification

<img width="1512" height="982" alt="Ekran Resmi 2026-06-29 15 40 39" src="https://github.com/user-attachments/assets/7c787205-f2a8-4316-873a-518252a56d2a" />


---

## Firewall Configuration

A firewall rule was created to allow inbound TCP traffic on port 8080.

### Screenshot - Firewall Rule

<img width="1512" height="982" alt="Ekran Resmi 2026-06-29 15 42 51" src="https://github.com/user-attachments/assets/17f89194-a921-47c1-aaf0-11f36d3a6e4c" />


---

## Public Access

The application was successfully accessed through the VM's public IP address.

Example:

```text
http://35.241.129.163:8080
```

### Screenshot - Public Access

<img width="1512" height="982" alt="Ekran Resmi 2026-06-29 15 40 46" src="https://github.com/user-attachments/assets/fcef0cf6-20de-41ab-bea2-8872eeaccf1f" />


---

## Result

The Nginx container was successfully deployed using Docker Compose on both a local machine and a Google Cloud VM.

The deployment was verified through:

- Docker container status checks (`docker ps`)
- Local browser access (`localhost:8080`)
- VM validation using `curl`
- Public access through the VM external IP address
- Google Cloud firewall configuration allowing inbound traffic on port 8080

The application was successfully reachable both locally and externally, confirming that the deployment was completed successfully.
