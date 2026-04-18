# Nginx + Redis Stack

A multi-container Docker Compose project running Nginx and Redis  together.

## Stack 

- *nginx* - web server serving static HTML
- *redis 7* - in-memory data store on port 6379

## Run

```bash
docker-compose up -d

```

## Check 

```bash
# Check nginx 
curl http://localhost:8080
```

```bash
# Check Redis
docker exec -it nginx-redis-redis-1 redis-cli ping
```
## Stop
```bash
docker-compose down
```

