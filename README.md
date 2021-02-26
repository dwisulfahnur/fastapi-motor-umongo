# Blog API with FastAPI

Simple project that I write using fastapi, motor, and umongo for the backend. VueJS on the frontend.

----------------------------
## Commands

### Run 
Run the app using the following command:
```
make up
```
or
```
docker-compose up -d --build
```


### Remove container
remove container

```
docker-compose down
docker-compose down -v --remove-orphans # delete all previous container and volume included
```
or
```
make down
make down-all
```

### Log Monitor

Monitor log for all services (mongodb, backend/api, frontend/vuejs)
```
docker-compose logs -f
```
or 
```
make logs
```

Monitor log for backend service only
```
docker-compose logs -f backend
```
or 
```
make logs-backend
```

### Run Test for the backend service
```
docker-compose exec backend pytest
```
or 
```
make test-backend
```

The API Documentation url:
http://127.0.0.1:8000/docs


The Blog:
http://127.0.0.1:8080