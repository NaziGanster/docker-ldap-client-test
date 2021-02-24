# docker-ldap-client-test
Test ldap client in docker

### Ldap Server
testldap:latest

### Ldap Client
testclient:latest

### Build Image And Run Test
docker compose will auto build image and start service
```
docker-compose -f docker-compose.yml up
```

test ldap client work well

```
#list start docker container and find client 
docker ps 


docker exec -it ${client_container_id} getent group
docker exec -it ${client_container_id} getent passwd
```
