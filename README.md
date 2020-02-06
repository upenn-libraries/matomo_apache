## README for `matomo_apache`

This is a Dockerized instance of Matomo running with Apache and a database client. 

### Requirements

* Docker 19.x or higher
* docker-compose 3.x or higher 

### Deployment 

From the root directory of the deployment repo, create your database config as follows:

```bash
cp db.env.example db.env
```

Replace the variable values with appropriate values for your database connection.

```bash 
docker stack deploy matomo_apache -c docker-compose.yml 
```


