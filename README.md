# rabbitmq-docker
Dockerized RabbitMQ

Docker build for RabbitMQ as per http://www.sysrun.io/2015/11/02/dockerize-rabbitmq/

---

** Usage **
  1. `docker build -t adsabs/rabbitmq .`
  1. `docker run -d --name rabbitmq -t -h rabbitmqhost -d -p 1883:1883 -p 15672:15672 -v
  /proj.adsqb/beer/rabbitmq-data:/var/lib/rabbitmq adsabs/rabbitmq`


In your run command, remember to provide persistant name and disk
volume so state isn't lost on restart.
