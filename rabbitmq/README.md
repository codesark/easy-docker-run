# Redis + Redis Commander (Docker Compose)

- Host: localhost, rabbitmq
- Network: rabbitmq-net 
- Port: 5672
- UI: http://localhost:10085
- UI User: `guest` | Password: `guest`

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
