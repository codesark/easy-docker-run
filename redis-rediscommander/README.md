# Redis + Redis Commander (Docker Compose)

- Host: localhost, redis
- Network: redis-net 
- Port: 6379
- UI: http://localhost:10083
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
