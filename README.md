# NGINX Load Balancer for 4 Backend Machines with manual commands of Docker

This project sets up an NGINX load balancer that distributes traffic across 4 backend servers.

## 🔧 Configuration File

- **File:** `load-balancer.conf`
- **Location (on server):** `/etc/nginx/conf.d/mysite.conf`

## 🧩 Backend Server IPs

```nginx
 upstream mybackend{
                server 127.0.0.1:32768;
                server 127.0.0.1:32769;
                server 127.0.0.1:32770;
                server 127.0.0.1:32771;
        }

