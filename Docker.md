# PORTAINER

docker volume create portainer_data

docker pull portainer/portainer-ce

docker run -d -p 8000:8000 -p 9000:9000 --name=portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data portainer/portainer-ce
************************************************************************

# RabbitMQ wManager

docker run -d -p 15672:15672 -p 5672:5672 --name RabbitMQContainer rabbitmq:3.8.14-management

************************************************************************

# MsSql

MacOS ile çalışmaktadır. 

docker pull mcr.microsoft.com/azure-sql-edge

docker run -e "ACCEPT_EULA=1" -e "MSSQL_SA_PASSWORD=Password12*" -e "MSSQL_PID=Developer" -e "MSSQL_USER=SA" -p 1433:1433 -d --name=sql mcr.microsoft.com/azure-sql-edge

************************************************************************
# Sonar Qube 

docker pull sonarqube
