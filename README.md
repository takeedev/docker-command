# Docker compose usage
[Link Docker Doc](https://docs.docker.com/reference/cli/docker/)

## Start docker daemon
### linux
```text
sudo systemctl start docker.
```
### mac
```text
docker desktop start
```
```text
open -a Docker
```


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

## Docker tag
```bash
docker tag source-image:tag target-image:tag
```

## Docker import image to .tar 
```bash
docker load -i image.tar or docker load < file.tar.zip 
```

## Docker save image to .tar
```bash
docker save -o filename.tar image-name:tag 
```
