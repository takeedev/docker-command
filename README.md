# Docker compose usage

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
