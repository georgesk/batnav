BATNAV fournit un serveur minimal, basé sur la bibliothèque Python3-cherrypy3

À l'origine, BATNAV était pensé pour pouvoir servir à créer un jeu de
bataille navale multi-joueurs.

Le projet n'évoluera pas beaucoup : il est juste censé offrir une base
pour de futurs développements, et éviter de perdre du temps à se demander
comment on peut :
* faire une session qui accompagne chaque joueur. Lors de chaque requête, le serveur doit pouvoir déterminer de quel joueur elle vient ;
* servir des données au format JSON avec l'en-tête normalisé qui va bien ;
* servir une page HTML prévue pour passer la validation du W3C, avec l'option « stricte ».

Quelques améliorations qui devraient pouvoir être faites sans trop de fatigue :
* lors de la création d'une nouvelle session, authentifier le joueur de façon forte ;
* créer une page de style particulière ;
* etc.

Ces améliorations ne se feront pas dans ce dépôt : le but de ce dépôt GIT est plutôt d'être utilisé dans un contexte d'apprentissage. Ce sont les étudiants qui font des améliorations, en créant des dérivés. 

## Licence : GPL V3

**Notez bien** : la licence des sources ici présentes vous oblige à placer les dérivés sous licence GPL V3.

## Mode d'emploi

Il faut que Python3 et python3-cherrypy3 soient installés sur la machine locale.

Quand on lance la commande ```python3 serveur.py``` un service web est créé, celui-ci répond à l'URL http://localhost:8080 par défaut. Selon les réglages du pare-feu, ce service est visible (ou non) des machines qui sont sur le même réseau local.
