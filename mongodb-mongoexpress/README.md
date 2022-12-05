# MongoDB + Mongo Express (Docker Compose)

- Host: localhost, mongo
- Network: mongo-net 
- Port: 27017
- UI: http://localhost:10082
- UI User: > `root` | Password: `toor`


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
