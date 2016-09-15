# Kubernetes


## Intérêt
* Orchestrer des containers<!-- .element: class="fragment" -->
 * déploiement dans un cluster<!-- .element: class="fragment" -->
 * service discovery / Load Balancing<!-- .element: class="fragment" -->
 * scale<!-- .element: class="fragment" -->
 * reprise sur crash<!-- .element: class="fragment" -->
 * rollouts / rollbacks<!-- .element: class="fragment" -->


## Vocabulaire
* <!-- .element: class="fragment" -->**Pod** : groupe de containers
* <!-- .element: class="fragment" -->**Replicaset** : permet de s'assurer qu'un ensemble de pods s'execute en même temps
* <!-- .element: class="fragment" -->**Service** : définition d'un ensemble de pods et de la manière dont on y accède
* <!-- .element: class="fragment" -->**Deployment** : permet de faire des mise à jours de versions...


## Démo
http://kubernetes.io/docs/hellonode/