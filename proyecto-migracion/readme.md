# Primer paso, convertir el docker compose a kubernetes instance
Para poder convertir el docker-compose se usa kompose se puede instalar desde https://kompose.io/

luego se usa el comando `kompose convert`

luego se ejecuta 

`kubectl apply -f rabbitmq-service.yaml`
`kubectl apply -f rabbitmq-deployment.yaml`

`kubectl apply -f db-service.yaml`
`kubectl apply -f db-deployment.yaml`

`kubectl apply -f api-service.yaml`
`kubectl apply -f api-deployment.yaml`

`kubectl apply -f listener-deployment.yaml`

para realizar la prueba se accede a la máquina del cluster

se obtiene la IP del service con kubectl get svc api

Se obtendría por ejemplo `10.105.192.60`

y se realiza curl 10.105.192.60