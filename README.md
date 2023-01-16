 [![Docker Image CI](https://github.com/alejunio/lemp-docker-compose/actions/workflows/docker-image.yml/badge.svg)](https://github.com/alejunio/lemp-docker-compose/actions/workflows/docker-image.yml)


# LEMP com Docker Compose Nginx PHP 7.4 e MySQL 8
## Ambiente de desenvolvimento PHP com Nginx e MySQL.

### Requisitos
* Docker
* Docker Compose



### Deploy Stack 
Para inicializar a Stack execute os passos abaixo

#### Clone o Repositório
```shell
git clone https://github.com/alejunio/lemp-docker-compose.git stack && cd stack
```

#### Iniciando a Stack em máquina local
```shell
docker-compose -f docker-compose-local.yml up -d 
```

#### Iniciando a Stack em VPS para utilizar SSL
```shell
docker-compose -f docker-compose-ssl.yml up -d 
```

Após inicializar a stack, acesse o Nginx Proxy Manager no navegador através da URL abaixo
```shell
http://ip_servidor:81

Email:    admin@example.com
Password: changeme
```




