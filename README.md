# cedar-docker-keycloak
Keycloak with Postgres

The content is based on:

https://github.com/jboss-dockerfiles/keycloak/tree/bfd9a115c4f630034461b6cca5f2048c43c222c2/server-postgres

## Building and pushing to DockerHub:

````
docker build -t cedar-keycloak-postgres .

docker login

docker tag cedar-keycloak-postgres metadatacenter/cedar-keycloak-postgres:1.0.6
docker push metadatacenter/cedar-keycloak-postgres:1.0.6

docker tag cedar-keycloak-postgres metadatacenter/cedar-keycloak-postgres:latest
docker push metadatacenter/cedar-keycloak-postgres:latest
````