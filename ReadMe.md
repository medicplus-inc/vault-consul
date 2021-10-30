# github.com/medicplus-inc/vault-consul

## Description
Infra tools to run vault and consul in docker container

## Dependencies

1. Docker v20.10.8
2. Docker-Compose v1.29.2
3. Vault v1.8.2
4. Consul v1.10.2

## How to run 

### To run the container:
1. Run command `$ docker-compose up -d --build`
2. Check logs `$ docker-compose logs`
3. initialized vault 
```
1. $ docker-compose exec vault bash
2. $ vault operator init
3. $ vault operator unseal (use unseal key #1)
4. $ vault operator unseal (use unseal key #2)
5. $ vault operator unseal (use unseal key #3)
6. $ vault login (use vault token)
```

## Credit
Michael Herman (https://testdriven.io/blog/managing-secrets-with-vault-and-consul/)
