# Docker compose usage
[Link Docker Doc](https://docs.docker.com/reference/cli/docker/)

## Start all service 
```bash
docker-compose up -d
```

## Start with specific compose file 
```bash
docker-compose -f loadtest-compose.yml up -d
```

## Start with multifile compose files 
```bash
docker-compose -p pref -f loadtest-compose.yml -f monitoring-compose.yml up -d
```

## Set project name 
```bash
docker-compose -p pref up -d
```

## Docker container exec 
```bash
docker exec -it {container-name or container-id} sh
```

## Docker copy file (host to container) 
```bash
docker cp /file.txt container-name:/path/container 
```

## Docker copy file (container to host)
```bash
docker cp container-name:/path/container /path/host 
```
