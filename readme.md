### Commands to run

```
docker-compose up -d
docker-compose exec superset superset-init
docker-compose down
```

### Services

1. Superset
2. Redis - Message broker
3. PostgreSQL - Metadata DB
4. Worker - Distibuted task queue based on Celery
5. Flower - Monitoring Celery workers


### Host ports

- Redis: 6379
- PostgreSQL: 5432
- Superset: 8088
- Flower: 5555

### Acknowledgements

Based on:
 - https://github.com/apache/incubator-superset/tree/master/contrib/docker
 - https://github.com/amancevice/superset