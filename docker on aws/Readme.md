
## Check Deployed docker container on AWS

```bash
sudo su
sudo service docker start
docker images
docker ps
```

go to browser and type - 

```bash
<your-aws-ec2-public-ip>:<app-port-number>

e.g.
http://34.229.181.52:7090/swagger-ui.html
```

## check postgreSQL database tables on docker

```
docker exec -it s3-postgresqldb-1 sh
psql -U postgres
\l
\c HomeInsuranceDatabase
\dt
select * from admin;
```
