# READ THIS FIRST

## Mandatory Steps

1. Create a docker network
2. Attach the traefik and other services to the network

## Mandatory Labels for Traefik

```md
traefik.enable=true
traefik.http.routers.service_name.entrypoints=web, websecure
traefik.http.routers.service_name.rule=Host(`service_name.example.com`)
traefik.http.routers.service_name.tls.certresolver=production
```
