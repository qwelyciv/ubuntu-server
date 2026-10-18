# Private Cloud & Telemetry Infrastructure

Automated deployment of a private cloud storage solution with a comprehensive observability stack, utilizing Nginx as a reverse proxy.

## Architecture
- **Reverse Proxy:** Nginx (Port 80)
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
2. Configure the environment variables by copying the template:
*(Edit `.env` to set your secure `DB_PASSWORD`)*
3. Run the Ansible playbook to provision the infrastructure:
4. **Local DNS Setup:** Map the application domains to your server's IP address (or `127.0.0.1` if using local port forwarding) in your client machine's `hosts` file (`/etc/hosts` or `C:\Windows\System32\drivers\etc\hosts`):
## Access Points
- **Nextcloud:** `http://cloud.local`
- **Grafana:** `http://grafana.local`
- **Prometheus:** `http://prometheus.local`
