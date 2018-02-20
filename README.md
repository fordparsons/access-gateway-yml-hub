access-gateway-x.x.x-letsencrypt adds TLS termination with automatic LetsEncrypt cert generation to the Duo Access Gateway. It incorporates the [jwilder/nginx-proxy](https://github.com/jwilder/nginx-proxy) and [jrcs/letsencrypt-nginx-proxy-companion](https://github.com/JrCs/docker-letsencrypt-nginx-proxy-companion) projects.

#Prerequisites

Docker, Docker-Compose

Two public DNS records will be needed for the Duo Access Gateway: one for its general use and another for its management interface. These will need to be added in the place holders in the  (.env) files.

A text file entitled with your management interface URL will need to be placed at /var/nginx/vhost.d/your.management.url with the contents:
listen 8443 ssl http2;

#Running

Follow the prereqs and Docker-Compose up at will!
