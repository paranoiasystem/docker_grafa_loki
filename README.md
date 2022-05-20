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

#### How call /loki Rest API

to call the Loki's Rest API that start with /loki you need to put ad extra /loki in url path

example: `http://localhost/loki/loki/api/v1/push`

it's useful in promtail config file