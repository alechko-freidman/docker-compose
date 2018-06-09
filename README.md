# Docker​-Compose -​ LEMP

* Containers:
    * Nginx
    * PHP-FPM
    * MySQL

### General

Use **docker.compose** template to create the above containers 
The stack does not contain wordpress, but only the infra needed for its deployment

### Prerequisites

Docker and Docker-Compose should be installed:

* Docker on RH/CentOS
```
sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo
sudo yum install docker-ce -y
```

* Docker-Compose
```
sudo pip install docker-compose
```

* To access test php file, add the server name your /etc/hosts file
```
<IP> php-docker.local
 ```

### Example

Run docker-compose
```
cd /dir/
docker-compose up -d
```
Browse to php test file
```
http://php-docker.local
```