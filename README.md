# docker-lemp

Run Nginx, php-fpm and MariaDB using [Docker]

## Requirements
Install [Docker] and [Compose]

## Usage
```
Clone the repository using the below command:

git clone https://github.com/gauravbhaskar84/ansible-test.git
cd ansible-test
docker-compose up -d  (to run in the background)
docker-compose logs (to check the logs)
docker-compose stop (to stop the containers)
docker-compose rm (to remove the containers)

docker container ls -a (to display running containers)
```

```
Please make sure that you have a hostname as architrave.local in your /etc/hosts file, otherwise http://localhost or whatever hostname you have for your hostname will serve the website. If it is there then http://architrave.local will work fine.

There are other steps as per Part 1 Test, whch is not required for the Docker Container, because we are not going to deal with the website that way. Website will only work for ports which are exposed by docker-compose.

http to https redirection does not work straight forward with docker, for that other steps are necessary.Example setting up a load-balancer with https URL and forwarding request to 1 or more docker application.
```

=====================

[Docker]:                      https://www.docker.io/
[Compose]:                     http://docs.docker.com/compose/install/
