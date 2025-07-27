# 🛡️ Privacy Docker Compose Setup

This guide walks you through setting up a privacy-focused Docker Compose stack using AirVPN, NGINX, and Transmission.

---

## 🌐 0. Configure AirVPN Account Settings

Before starting, follow this visual guide to properly configure your AirVPN settings:

📸 [AirVPN Setup Guide](https://github.com/laosmidas/deb-omv-dots/tree/main/docker_compose_examples/privacy/airvpn_settings)

---

## 📁 1. Copy NGINX Directory

Copy the `nginx` directory into your `privacy` folder:

🔗 [nginx directory](https://github.com/laosmidas/deb-omv-dots/tree/main/docker_compose_examples/privacy/nginx)

---

## 🔐 2. Generate Certificates for Mullvad Browser

Follow these instructions to create self-signed certificates for secure browser use:

📄 [Certificate Guide](https://github.com/laosmidas/deb-omv-dots/blob/main/docker_compose_examples/privacy/selkies-certs/RUN_COMMANDS.md)

---

## ⚙️ 3. Configure `docker-compose.yml`

Edit your `docker-compose.yml` file based on the AirVPN example (recommended for privacy):

📄 [docker-compose_example_airvpn.yml](https://github.com/laosmidas/deb-omv-dots/blob/main/docker_compose_examples/privacy/docker-compose_example_airvpn.yml)

---

## 🚀 4. Launch the Docker Stack

Use the following commands in your terminal to start the stack:

```bash
docker compose pull
docker compose up -d
```

---

## 🧭 5. Configure Transmission Application

After launching, adjust the Transmission settings by referring to this visual guide:

📸 [Transmission Settings Guide](https://github.com/laosmidas/deb-omv-dots/tree/main/docker_compose_examples/privacy/transmission_settings)

---

## 🌍 6. Access Web Interfaces

- 📦 **Transmission**  
  Visit: `http://localhost:9091`

- 🔐 **Mullvad Browser (via noVNC)**  
  Visit: `https://localhost:6901`

> Replace `localhost` with your server's IP if accessing remotely.

---
