 [![Docker Image CI](https://github.com/alejunio/lemp-docker-compose/actions/workflows/docker-image.yml/badge.svg)](https://github.com/alejunio/lemp-docker-compose/actions/workflows/docker-image.yml)


# LEMP com Docker Compose Nginx PHP 7.4 e MySQL 5.7
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

#### Depploy Stack
```shell
docker-compose up -d
```


### Estrutura

.
├── LICENSE
├── README.md
├── app
│   └── info.php
├── conf
│   └── app.conf
├── docker-compose.yml
├── mysql
│   ├── Dockerfile
│   └── docker-entrypoint.sh
└── nginx
    ├── 10-listen-on-ipv6-by-default.sh
    ├── 20-envsubst-on-templates.sh
    ├── Dockerfile
    └── docker-entrypoint.sh