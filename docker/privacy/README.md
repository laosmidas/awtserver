# 🛡️ Privacy Docker Compose Setup

This guide walks you through setting up a privacy-focused Docker Compose stack using AirVPN, NGINX, and Transmission.

---

## 🌐 1. Configure AirVPN Account Settings

Before starting, follow this visual guide to properly configure your AirVPN settings:

📸 [AirVPN Setup Guide](https://github.com/laosmidas/deb-omv-dots/tree/main/docker_compose_examples/privacy/airvpn_settings)

---

## ⚙️ 2. Configure `docker-compose.yml`

Edit your `docker-compose.yml` file based on the AirVPN example (recommended for privacy):

📄 [docker-compose_example_airvpn.yml](https://github.com/laosmidas/deb-omv-dots/blob/main/docker_compose_examples/privacy/docker-compose_example_airvpn.yml)

This service expects TLS certs to be mounted into the container. Use an **absolute path** on your host. Details and folder layout:  
[deb-omv-dots/docker/tailscale-certs](https://github.com/laosmidas/deb-omv-dots/tree/main/docker/tailscale-certs)

---

## 🚀 3. Launch the Docker Stack

Use the following commands in your terminal to start the stack:

Pull Updates for docker apps
```bash
sudo docker compose pull
```
Launch docker stack
```bash
sudo docker compose up -d
```

---

## 🌍 4. Access Web Interfaces

- 📦 **Transmission**  
  Visit: `https://localhost:6091/transmission/`

- 🔐 **Mullvad Browser (via noVNC)**  
  Visit: `https://localhost:6901/browser/`

> Replace `localhost` with your server's IP if accessing remotely.

---

## 🧭 5. Configure Transmission Application

After launching, adjust the Transmission settings by referring to this visual guide:

📸 [Transmission Settings Guide](https://github.com/laosmidas/deb-omv-dots/tree/main/docker_compose_examples/privacy/transmission_settings)

---
