
## Monitorando Aplicação com Prometheus & Grafana



## APP NodeJs

Comandos iniciar aplicação em NodeJs

* npm start
* node index.js

## Prometheus - Docker
* Iniciar container Docker com o Prometheus
* docker run
  -- name prometheusandgrafan
  -- rm
  -d
  -p 
  -v /home/prometheus.yml:/etc/prometheus/prometheus.yml
  prom/prometheus

* docker run --name prometheus --rm -d -p 9090:9090 -v /home/prometheus.yml:/etc/prometheus/prometheus.yml prom/prometheus

* Acessar via http://localhost:9090

## Grafana - Docker

* Iniciar container Docker com o Grafana
* docker run -d --name=grafana -p 3000:3000 grafana/grafana
* Acessar via http://localhost:3000

## Docker Compose

* Iniciar container Docker com o Prometheus e Grafana através do arquivo docker-compose.yml

* docker-compose up
