# Auth

## Getting started

1. Install [Docker](https://www.docker.com/get-docker)
1. `docker volume create pgauth`
1. Clone code
1. `docker-compose up -d database`
1. `docker-compose run auth "-Dkeycloak.migration.action=import -Dkeycloak.migration.strategy=OVERWRITE_EXISTING -Dkeycloak.migration.provider=dir"`
1. `docker-compose up -d`
1. Navigate to http://localhost:30303/auth/admin/master/console/#/
1. Log in with admin:admin