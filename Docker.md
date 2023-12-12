# PORTAINER

docker volume create portainer_data

docker pull portainer/portainer-ce

docker run -d -p 8000:8000 -p 9000:9000 --name=portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data portainer/portainer-ce
************************************************************************

# RabbitMQ wManager

docker run -d -p 15672:15672 -p 5672:5672 --name RabbitMQContainer rabbitmq:3.8.14-management

************************************************************************

