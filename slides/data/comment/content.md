## Ok... A quoi ça va me servir ?
![solution-code](data/comment/how.gif)<!-- .element: style="width:100%" -->


## Commment Docker répond au pb ?
 * <!-- .element: class="fragment" -->faire des technos **différentes** sur des environnements **différents**
 * <!-- .element: class="fragment" -->**isolation** du container. Facilite la configuration réseau, disque, ...
 * <!-- .element: class="fragment" -->**automatisation** : opération standards et scriptables pour démarrer / stopper ... un container
 * <!-- .element: class="fragment" -->**Performances** : peu d'overload
 * <!-- .element: class="fragment" -->séparation des **responsabilités** : les devs s'occupent du code, les ops s'occupent de l'infra


## Intérêts pour les Dévs
 * <!-- .element: class="fragment" -->on **build une fois** / on déploie sur tous les environnements (dev/recette/prod)
 * <!-- .element: class="fragment" -->possibilité de prendre une **snapshot** d'un container pour le redémarrer ailleurs
 * <!-- .element: class="fragment" -->pas de problèmes de **conflits** entre 2 applications
 * <!-- .element: class="fragment" -->on peut **automatiser** le déploiement, les tests, etc...
 * <!-- .element: class="fragment" -->réduit les **différences** entre les environnements

Note: on a déjà tous eu un pb reproduit uniquement en recette car l'environnement n'était pas configuré comme la dev.


## Intérêts pour les ops
 * <!-- .element: class="fragment" -->Il suffit d'installer **docker** pour faire tourner n'importe qu'elle application
 * <!-- .element: class="fragment" -->**Environnements** de dev/rec/prod **identiques**
 * <!-- .element: class="fragment" -->Améliore le **temps de mise en place** des environnements
 * <!-- .element: class="fragment" -->Plus **performant** qu'une VM
 * <!-- .element: class="fragment" -->Règle la plupart des problèmes d'**isolation**


## Différence entre VM et Container
 * Pas de Guest OS à charger.
 * Librairies partagées.
![containers-vs-vms](data/comment/containers-vs-vms.png)
 * démarre rapidement
 * moins gourmand en resources
