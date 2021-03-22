# README

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/OlivierNalin/myBinderBigQ/HEAD)

La DIRIF examine plusieurs solutions pour faire des requêtes dans la base de données des trafics et vitesses qui sont enregistrés par les stations de comptage.
L'une des solution serait de charger les données dans un CLoud (Google BigQuery par exemple) et de faire des traitements standardisés par l'intermédiaires de "Jupyter notebooks".

L'exigence est que la solution permette à des techniciens de faire les opérations usuelles, sans maitriser la programmation des notebooks.

Pour vérifier la faisabilité de la méthode, j'ai chargé, dans une base BigQuery, les débits de toute l'année 2019 de 150 stations SIRIUS. J'ai créé un premier notebook qui permet à un utilisateur de sélectionner un axe (A13-W par exemple) dans une liste déroulante, puis de selectionner l'une des stations de cet axe ('A13-W/03+0400/P' par exemple), par une seconde liste déroulante. Après cela, l'utilisateur choisit les dates de début et de fin de l'extraction.

Pour lancer le notebook en ligne, on pourra utiliser l'outil Binder en cliquant sur l'icone :[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/OlivierNalin/myBinderBigQ/HEAD)

Le chargement peut prendre plusieurs minutes à la première utilisation.

Il sera possible d'ajouter le choix des jours de la semaine, le calcul du profil horaire moyen ou de toute autre statistique souhaitée.

L'avantage de cette solution est que l'évolution de l'application peut être réalisée par un "datascientist" et non par toute une équipe de développeurs informatiques.
Le cout de la prestation sera fortement réduit.

Dans la mesure où, la base de donnée peut être alimentée en temps réel, cette solution permettrait de prototyper des services complémentaires de surveillance du réseau.


