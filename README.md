# CICD System

Continuous Integration (CI) - Continuous Deployment (CD) System.

### Infrastructure Diagram

![Infrastructure diagram](diagrams/infrastructure-diagram.png)

### SonarQube

Administrator console is available to the following url:

`http://<MACHINE_IP>:9000`
	
Administrator credentials:

`USERNAME: admin`

`PASSWORD: admin`

Access token:

`jenkins: 7c7b358a089ccdc5367d6af77985ba0eac8ceb7f`

Maven goal:

```
mvn sonar:sonar
-Dsonar.host.url=http://sonarqube:9000
-Dsonar.login=7c7b358a089ccdc5367d6af77985ba0eac8ceb7f
```

### Jenkins

To show the initialAdminPassword, run command:

`docker exec <CONTAINER_ID> cat /var/jenkins_home/secrets/initialAdminPassword`

Admin console at following url:

`http://<MACHINE_IP>:8080`
	
Jenkins user:

`USERNAME: admin`

`PASSWORD: admin`

## Run infrastructure

`docker-compose up --build`

with **-d** option run all in detached mode
