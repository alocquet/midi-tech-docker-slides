# Next step : Docker compose


## Intérêt
* Démarrer une application avec plusieurs containers Docker
* Décrit toute l'architecture d'une application
* Démarrage de tous les containers en une seule commande

## Fichier Docker Compose
* depends_on : ordre de démarrage
* links : container A est visible par container b
* build : décrit comment construire une image
* image : nom de l'image
* environment : variables d'environnement
* command : commande à lancer dans le container
* port : forwarder un port
* volumes : définir des volumes


## config
Permet de lire et valider un fichier compose
```sh
docker-compose config
```


## create
Permet de créer les containers
```sh
docker-compose create [SERVICE...]
```


## (re)start
Permet de (re)démarrer les containers existant
```sh
docker-compose start  [SERVICE...]
docker-compose restart  [SERVICE...]
```


## up
up = create + start
```sh
docker-compose up -d [SERVICE...]
```


## ps
Lister les containers
```sh
docker-compose ps
```


## Logs
Lire les logs des containers
```sh
docker-compose logs [SERVICE...]
```


## pause
Pause les containers
```sh
docker-compose pause [SERVICE...]
```


## unpause
Relance les containers en pause
```sh
docker-compose unpause [SERVICE...]
```


## stop
Stopper les containers
```sh
docker-compose stop [SERVICE...]
```


## rm
Supprimer les containers
```sh
docker-compose rm [SERVICE...]
```


## down
down = stop + rm
```sh
docker-compose down  [SERVICE...]
```


## scale
Permet de définir le nombre de containers pour un service
```sh
docker-compose -f docker-compose-lb scale services=2
```
