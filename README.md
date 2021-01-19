# Docker-compose files for a simple uptodate
# InfluxDB
# + Grafana stack
# + Telegraf
# +spring boot app
# + mongoDb
# + elasticsearch
# + nginx
# + php-fpm

Get the stack (only once):

```
git clone https://github.com/ekzestencial/monitoring-system.git
cd monitoring-system
```

Run your stack:

```
sudo mkdir -p /srv/docker/grafana/data
docker-compose up -d
sudo chown -R 472:472 /srv/docker/grafana/data

```

Show me the logs:

```
docker-compose logs
```

Stop it:

```
docker-compose stop
docker-compose rm
```

Update it:
```

If you want to run Telegraf, edit the telegraf.conf to yours needs and:

```
docker exec telegraf telegraf
```
