
docker network create --driver=overlay traefik-public


mkdir -p /home/ubuntu/traefik
touch /home/ubuntu/traefik/acme.json
chmod 600 /home/ubuntu/traefik/acme.json
