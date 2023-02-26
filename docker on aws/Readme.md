
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
