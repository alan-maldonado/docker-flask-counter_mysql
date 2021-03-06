# Docker Compose

## Build the images
```bash
docker-compose build
```

## Run the containers
```bash
docker-compose up
```

## Init the db
```bash
docker exec -it counterapp_web_1 python dbinit.py
```

## To use the app container
```bash
docker exec -it counterapp_web_1 /bin/bash
```

## To use the mysql server
```bash
docker exec -it counterapp_db_1 mysql -uroot -prootpass
```

## Run tests
```bash
docker exec -it counterapp_web_1 python tests.py
```

## Start or stop containers
```bash
docker-compose start
docker-compose stop
```

## Remove the containers
```bash
docker-compose rm -v
```
