# monitoring-zabbix
Monitoring with Zabbix 6

## pull the images with podman
`podman image pull postgres:14.5-alpine`
`podman image pull zabbix/zabbix-server-pgsql:alpine-6.2-latest`
`podman image pull zabbix/zabbix-web-nginx-pgsql:alpine-6.2-latest`
`podman image pull zabbix/zabbix-agent2:alpine-6.2-latest`

## create a pod
`podman pod create --name pod-zabbix -p 8080:80 -p 10051:10051`

## create the database container
