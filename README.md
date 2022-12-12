# Easy Docker Run
Docker Compose files for quickly starting most commonly used services for development use. 

## Services

- PostgreSQL + PgAdmin
- MongoDB + Mongo Express
- Redis + Redis Commander
- Elasticsearch + Kibana

## Instructions

- Make sure you have docker and docker-compose installed
    - [Docker Desktop](https://docs.docker.com/get-docker/)
- Clone the repo using git `git clone https://github.com/codesark/easy-docker-run.git`
- Change the directory to cloned repo `cd easy-docker-run`
- Depending upon which service you want to run, **change to that directory** and run `docker-compose up -d` \
  and to stop run 'docker-compose down' or `docker compose down -v` to also remove the volumes \
  For Example:
    - To start: Postgres + PgAdmin 
       ```
       cd postgresql-pgadmin
       docker-compose up -d
       ```
      Above Commands will start configure and start the services using docker and docker compose
    - To stop: Postgresql + PgAdmin
       ```
       cd postgresql-pgadmin
       docker-compose down
       ```
 
 ## Contribution
 
 Feel free to add more services to the repo by forking the repo or creating a pull request directly. 
