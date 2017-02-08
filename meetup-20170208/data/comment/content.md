## Ok... A quoi ça va me servir ?
![solution-code](data/comment/how.gif)<!-- .element: style="width:100%" -->


## Commment Docker répond au pb ?
 * <!-- .element: class="fragment" -->des technos **différentes** sur des environnements **différents**
 * <!-- .element: class="fragment" -->**isolation** du container. Facilite la configuration réseau, disque, ...
 * <!-- .element: class="fragment" -->**automatisation** : opération standards et scriptables pour démarrer / stopper ... un container
 * <!-- .element: class="fragment" -->**Performances** : peu d'overload


## Intérêts pour les Dévs
 * <!-- .element: class="fragment" -->on **build une fois** / packaging facilité
 * <!-- .element: class="fragment" -->pas de problèmes de **conflits** entre 2 applications (librairies, configurations)
 * <!-- .element: class="fragment" -->on peut **automatiser** plus facilement
 * <!-- .element: class="fragment" -->réduit les **différences** entre les environnements


## Intérêts pour les ops
 * <!-- .element: class="fragment" -->Il suffit d'installer **docker** pour faire tourner une application
 * <!-- .element: class="fragment" -->**Environnements** de dev/rec/prod **similaires**
 * <!-- .element: class="fragment" -->Améliore le **temps de mise en place** des environnements
 * <!-- .element: class="fragment" -->Plus **performant** qu'une VM
 * <!-- .element: class="fragment" -->Règle la plupart des problèmes d'**isolation**


## Différence entre VM et Container
 * Pas de Guest OS à charger.
 * démarre rapidement
 * moins gourmand en resources
![containers-vs-vms](data/comment/containers-vs-vms.png)
