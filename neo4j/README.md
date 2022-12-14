# Redis + Redis Commander (Docker Compose)

- Host: localhost, neo4j
- Network: neo4j-net 
- Port: 7687
- UI: http://localhost:10086
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
