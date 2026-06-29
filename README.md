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

<img width="1512" height="982" alt="Ekran Resmi 2026-06-29 15 29 35" src="PASTE_LOCAL_DEPLOYMENT_IMAGE_LINK_HERE" />

### Screenshot - Local Browser Access

<img width="1161" height="408" alt="Ekran Resmi 2026-06-29 14 43 36" src="PASTE_LOCAL_BROWSER_IMAGE_LINK_HERE" />

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

<img width="1512" height="982" alt="Ekran Resmi 2026-06-29 15 40 39" src="PASTE_VM_DEPLOYMENT_IMAGE_LINK_HERE" />

### Screenshot - VM Verification

<img width="1512" height="982" alt="Ekran Resmi 2026-06-29 14 44 26" src="PASTE_VM_VERIFICATION_IMAGE_LINK_HERE" />

---

## Firewall Configuration

A firewall rule was created to allow inbound TCP traffic on port 8080.

### Screenshot - Firewall Rule

<img width="1512" height="982" alt="Ekran Resmi 2026-06-29 15 42 51" src="PASTE_FIREWALL_IMAGE_LINK_HERE" />

---

## Public Access

The application was successfully accessed through the VM's public IP address.

Example:

```text
http://35.241.129.163:8080
```

### Screenshot - Public Access

<img width="1512" height="982" alt="Ekran Resmi 2026-06-29 15 40 46" src="PASTE_PUBLIC_ACCESS_IMAGE_LINK_HERE" />

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
