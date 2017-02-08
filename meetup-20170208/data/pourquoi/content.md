## Quelques indicateurs
- github <!-- .element: class="fragment" -->
 - 3127 watchers
 - 39,486 stars
 - 11,843 forks
- docker hub <!-- .element: class="fragment" -->
 - fin 2016 : &gt; 6,000,000,000 pulls
 - 1 milliard toutes les 6 semaines


## Quelques indicateurs
![pulls](data/pourquoi/pull.png)


## Quelques indicateurs
![pulls](data/pourquoi/pull-2017.jpg)


![pulls](data/pourquoi/why.gif)<!-- .element: style="width:100%" -->


## Pb : Hétérogénéité
- Technologies
 - statique : nginx/apache, conf openssl, css, js<!-- .element: class="fragment" -->
 - appli web : jetty/tomcat, REST/SOAP<!-- .element: class="fragment" -->
 - bdd : postgresql/mysql, pgadmin/mysql<!-- .element: class="fragment" -->
 - batch : sh, python<!-- .element: class="fragment" -->
 - queues : redis<!-- .element: class="fragment" -->
- Déploiement<!-- .element: class="fragment" -->
 - local : dev<!-- .element: class="fragment" -->
 - cloud : AWS, Azure<!-- .element: class="fragment" -->
 - cluster de production on premise<!-- .element: class="fragment" -->
 - rpi<!-- .element: class="fragment" -->


## Pb : Hétérogénéité
![heterogeneite](data/pourquoi/heterogeneite.jpg)


## Pb : Hétérogénéité
* Comment gérer les dépendances 
* Comment éviter X configs différentes <!-- .element: class="fragment" -->
* Comment migrer/scaler rapidement une appli <!-- .element: class="fragment" -->


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


## pour nous
![solution-code](data/pourquoi/shipping-container-for-code.png)


## La matrice devient plus simple
![matrice-simple](data/pourquoi/eliminates-matrix-from-hell.png)
