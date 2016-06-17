## Quelques indicateurs
- github <!-- .element: class="fragment" -->
 - 2689 watchers
 - 32,009 stars
 - 9,170 forks
- docker hub <!-- .element: class="fragment" -->
 - &gt; 2,000,000,000 pulls
 - 7,000 pulls / minute
 - 20% sur l'un des 93 repos officiels


## Quelques indicateurs
![pulls](data/pourquoi/pull.png)


![pulls](data/pourquoi/why.gif)<!-- .element: style="width:100%" -->


## Evolution technos
* Avant : client lourd <!-- .element: class="fragment" -->
* Maintenant : archi plus complexe : <!-- .element: class="fragment" -->
 * Comment gérer les dépendances
 * Comment éviter X configs différentes
 * Comment migrer/scaler rapidement une appli.


## Pb : Hétérogénéité
![heterogeneite](data/pourquoi/heterogeneite.jpg)
Note:
## technologies
- statique : nginx, openssl, css, js
- appli web : jetty, tomcat, spring, REST
- bdd : Postgresql, pgadmin
- batch : sh, python
- queues : redis
## serveurs
- local : developpement
- cloud
- cluster de production


## Matrice
![matrice](data/pourquoi/matrice.png)


## Transport Cargo avant 1960
![cargo](data/pourquoi/cargo-transport-pre-1960.png)


## Même problème
![matrice2](data/pourquoi/matrice-2.png)


## Solution adoptée
![solution](data/pourquoi/ship-container.png)
Note:
Pour minimiser le cout de transport des marchandises, nous avons créé les conteneurs.


## mais encore...
![solution-code](data/pourquoi/cest-cela.gif)<!-- .element: style="width:100%" -->


## adaptation au code
![solution-code](data/pourquoi/shipping-container-for-code.png)


## La matrice devient plus simple
![matrice-simple](data/pourquoi/eliminates-matrix-from-hell.png)
