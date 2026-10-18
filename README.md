# Private Cloud & Telemetry Infrastructure

Automated deployment of a private cloud storage solution with a comprehensive observability stack using Docker Compose and Ansible.

## Architecture
- **App Tier:** Nextcloud
- **Database & Cache:** PostgreSQL, Redis
- **Telemetry & Monitoring:** Prometheus, Grafana, Node Exporter, cAdvisor
- **Security:** UFW (Firewall), Fail2ban

## Prerequisites
- Ubuntu Server
- Docker & Docker Compose
- Ansible

## Quick Start
1. Clone this repository.
2. Configure the environment variables by copying the example file:
*(Edit `.env` to set your secure `DB_PASSWORD`)*
3. Run the Ansible playbook to provision the infrastructure:
## Access Points
- **Nextcloud:** `http://<server-ip>:8080`
- **Grafana:** `http://<server-ip>:3000`
- **Prometheus:** `http://<server-ip>:9090`
