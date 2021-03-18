# Docker Proof of Concept: ReactJS App - Nginx Proxy - k8s

## Docker

Tested with 
- `docker` *version* `20.10.5`
- `docker-compose` *version* `1.28.5` 

on *Debian GNU/Linux 10 (buster)*

```bash
docker-compose build
docker-compose up -d
# open browser http://localhost/
```

## *k8s* files

Download `kompose`. See [url](https://kubernetes.io/docs/tasks/configure-pod-container/translate-compose-kubernetes/)

```bash
# run this command on the same folder where is docker-compose.yml
kompose convert
```

Will be created these files: *deployment* and *service* files for *k8s*

```bash
poc-nginx-proxy-deployment.yaml
poc-nginx-proxy-service.yaml
poc-reactjs-app-deployment.yaml
poc-reactjs-app-service.yaml
```
