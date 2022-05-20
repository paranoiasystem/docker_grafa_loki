# Docker + Grafana + Loki

A simple config for running grafana and loki on docker behind a nginx reverse proxy

## Default credential

### Grafana

admin:admin

after the first login, grafana gives you the possibility to change the password

### Loki

loki:loki

to change the configured Loki's auth password modify the file under /nginx/conf.d/loki.htpasswd

reference: https://docs.nginx.com/nginx/admin-guide/security-controls/configuring-http-basic-authentication/