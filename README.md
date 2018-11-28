# MySQL + Adminer on Docker container
My MySQL server for development purpose with Adminer.

## Usage
After clone, type this on the repository folder.
```
docker-compose up -d
```

It will run MySQL latest with Adminer for managing tables.

Adminer available through random http port. You can see it by typing `docker ps`. Here is the example.
```
CONTAINER ID        IMAGE               COMMAND                  CREATED             STATUS              PORTS                     NAMES
e30ed195ff33        adminer             "entrypoint.sh docke…"   41 minutes ago      Up 2 minutes        0.0.0.0:32773->8080/tcp   adminer-development
f97221745463        mysql:latest        "docker-entrypoint.s…"   41 minutes ago      Up 2 minutes        3306/tcp, 33060/tcp       mysql-development
```

On above example, Adminer available on port `32772` so you can go to `http://localhost:32773` to access Adminer.

Thank you.
