## Pratique
* <!-- .element: class="fragment" -->**Image** - Ensemble d'un filesystem et de paramètres d'éxecution. N'a pas d'état et est immuable
* <!-- .element: class="fragment" -->**Container** - Instance d'une image
* <!-- .element: class="fragment" -->**Dockerfile** - Script pour créer une image
* <!-- .element: class="fragment" -->**Index** - Registre d'images Docker
* <!-- .element: class="fragment" -->**Push / Pull** - Commandes pour charger ou créer des images dans l'index
* <!-- .element: class="fragment" -->**Run** - Démarrer une image dans un nouveau container


## Démo
* docker run -d -p 80:80 --name iamfoo emilevauge/whoami
* docker ps
* ps aux | grep ...


## La suite...
* <!-- .element: class="fragment" -->composition
 * <!-- .element: class="fragment" -->docker compose
 * <!-- .element: class="fragment" -->Démarrer un ensemble de containers
 * <!-- .element: class="fragment" -->Avec des liens entre eux
* <!-- .element: class="fragment" -->cluster
 * <!-- .element: class="fragment" -->Kubernetes, Docker swarm, AWS ECS
 * <!-- .element: class="fragment" -->Gérer un cluster de containers
 * <!-- .element: class="fragment" -->Scaler facilement
 * <!-- .element: class="fragment" -->Voir l'état du cluster
 * <!-- .element: class="fragment" -->Gérer le failover, les montées de version, ...
* <!-- .element: class="fragment" -->Autres : Rancher, traefik, ...