# change-data-capture-example
A CDC(Change Data Capture) example Between PostgreSQL and Couchbase DB

Start using with command.
```sh
docker compose up -d  
```

## PostgreSQL related Commands
Open shell in Postgresql Container using container name as `postgres` . (Find container ID using `docker ps` command).
```sh
docker exec -it postgres /bin/bash
```

Use psql command to connect to PostgreSQL as `debezium` user and `mydb` database.
```sh
psql -U debezium -d mydb
```

List Databases in PostgreSQL.
```psql
\l
```

Connect to `POSTGRES_DB: new_db` as declared in `postgresql.yaml` file.
```psql
\c mydb
```

Check values in users table.
```sql
SELECT * FROM users;
```