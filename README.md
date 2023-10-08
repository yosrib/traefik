
## Traefik


docker network create --driver=overlay traefik-public
docker network create --driver=overlay pma-public
docker network create --driver=overlay db-server


mkdir -p /home/ubuntu/traefik
touch /home/ubuntu/traefik/acme.json
chmod 600 /home/ubuntu/traefik/acme.json

## Generate password
openssl passwd -apr1

openssl rand -base64 20


## Volumes


## References
### Traefik
https://dockerswarm.rocks/traefik/

### Volume
https://thenewstack.io/tutorial-create-a-docker-swarm-with-persistent-storage-using-glusterfs/
