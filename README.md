# Monitoring Nginx availability using Prometheus, Alertmanager and Blackbox exporter


1. Install docker on the workstation. see the link for details https://docs.docker.com/get-docker/
2. Install docker-compose. see https://docs.docker.com/compose/install/
3. clone this repository
```
  git clone https://github.com/popsonebz/monitoring.git
```
4. change directory to the cloned repo.
On Linux or Mac OS
```
  cd monitoring
```
5. Ensure you are connected to the internet to execute this command.
```
  docker-compose up -d
```
6. check if the docker containers are up.
```
  docker ps
```
You should see the following if all works well.

![Screenshot](https://github.com/popsonebz/monitoring/blob/main/images/monitoring-nginx.png)
7. Verify the services are running using the browser.
  a. prometheus: http://localhost:9090
  ![Screenshot](https://github.com/popsonebz/monitoring/blob/main/images/prometheus.png)
  b. alertmanager: http://localhost:9093
  ![Screenshot](https://github.com/popsonebz/monitoring/blob/main/images/alertmanager.png)
  c. nginx:  http://localhost:8080
  ![Screenshot](https://github.com/popsonebz/monitoring/blob/main/images/nginx.png)
