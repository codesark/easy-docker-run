# Elasticsearch + Kibana (Docker Compose)

- Host: localhost, postgres
- Network: elasticsearch-net 
- Port: 9200
- UI: http://localhost:10084
- UI User: `<n/a>` | Password: `<n/a>`

## Create/Start
```shell
# Start 
docker-compose up

# Start in Backgroud (as daemon)
docker-compose up -d
```

## Stop/Remove
```shell
# Stop + Remove Networks
docker-compose down

# Stop + Remove Networks + Remove Containers
docker-compose down -v
```
