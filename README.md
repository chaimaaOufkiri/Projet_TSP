# Projet Métaheuristiques : TSP

Ce projet porte sur la résolution du **Problème du Voyageur de Commerce (TSP)**. Nous avons implémenté et comparé des algorithmes allant du plus simple (Glouton) au plus complexe (Recherche Tabou).

## Organisation des fichiers

Le projet est structuré comme suit :

* **`Projet.ipynb`** : C'est le fichier principal. Il contient tout le code, les tests sur les instances, les comparaisons et l'analyse des résultats.
* **`instances/`** : Ce dossier contient les fichiers de données (.tsp) comme `st70`, `pr1002`, etc., qui servent de base à nos tests.
* **`src/`** : Ce dossier contient les scripts Python qui font tourner les algorithmes :
    * `heuristique.py` : L'algorithme du Plus Proche Voisin (PPV).
    * `metaheuristique.py` : L'algorithme de la Recherche Tabou.
    * `utils.py` : Fonctions pour lire les fichiers et calculer les distances.
    * `synthese_resultats_TSP.csv` : Fichier contenant l'intégralité des mesures (coûts et temps) obtenues lors des tests.
    

##  Ce que nous avons fait

1. **Approche Gloutonne (PPV)** : Nous avons commencé par une solution rapide qui choisit toujours la ville la plus proche.
2. **Recherche du meilleur départ** : Nous avons testé l'algorithme PPV en changeant la ville de départ pour trouver la meilleure base possible.
3. **Recherche Tabou** : Nous avons optimisé la solution précédente en utilisant une méthode qui explore le voisinage (2-opt) et évite de revenir en arrière grâce à une "liste tabou".

## Comment lire les résultats ?

Tout est prêt à l'emploi dans le Notebook. Les résultats sont affichés sous forme de tableaux comparatifs et de graphique montrant l'évolution du coût de la tournée.
