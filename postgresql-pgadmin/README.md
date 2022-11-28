# PostgreSQL + PgAdmin (Docker Compose)

- Host: localhost, postgres
- Network: postgres-net 
- Port: 5432
- UI: http://localhost:10081
- UI User: postgres@pgadmin.org | Password: postgres

## Create/Start
```shell
# Start 
docker-compose up

# Start in Backgroud (as daemon)
docker-compose up -d
```

# Stop/Remove
```shell
# Stop + Remove Networks
docker-compose down

# Stop + Remove Networks + Remove Containers
docker-compose down -v
```