# Docker-compose files for a simple uptodate
# InfluxDB
# + Grafana stack
# + Telegraf

Get the stack and create volumes (only once):

```
git clone https://github.com/josteinbf/docker-influxdb-grafana.git
cd docker-influxdb-grafana
docker volume create influxdb-storage
docker volume create grafana-storage
```

Run your stack:

```
docker-compose up -d

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

Modify version numbers in docker-compose.yml to your liking, then stop and restart.


If you want to run Telegraf, edit the telegraf.conf to yours needs and restart the stack.

