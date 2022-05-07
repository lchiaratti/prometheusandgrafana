
## Monitorando Aplicação com Prometheus & Grafana

## APP

* Comandos iniciar aplicação

npm start
node indes.js

## Prometheus - Docker
docker run
  -- name prometheusandgrafan
  -- rm
  -d
  -p 
  -v /home/prometheus.yml:/etc/prometheus/prometheus.yml
  prom/prometheus

docker run --name prometheus --rm -d -p 9090:9090 -v /home/prometheus.yml:/etc/prometheus/prometheus.yml prom/prometheus

## Grafana - Docker

docker run -d --name=grafana -p 3000:3000 grafana/grafana

## Docker Compose

docker-compose up