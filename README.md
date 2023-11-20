# Pokemon-recommender
A recommender system using Machine Learning classification with KNN algorithm.

## Objectif
Maitriser les notions de distance
Utiliser le KNN pour trouver des similarités

## Challenge
Un champion du monde Pokémon (oui, cela existe) a entendu parler de tes connaissances en Machine Learning et demande ton expertise.

Le champion a l'habitude d'utiliser les Pokemon suivants : Mewtwo, Lugia, Rayquaza, Giratina, Dialga, et Palkia. Mais pour sa prochaine compétition, il est interdit d'utiliser un Pokémon légendaire. Un pokemon est soit légendaire, soit non-légendaire. La dernière colonne du dataset indique True ou False suivant les cas.
Le champion devra donc remplacer ses Pokemon légendaires préférés par d'autres Pokémons non-légendaires, avec des caractéristiques similaires. C'est là que tu interviens !

Pour l'aider, suis les étapes suivantes :

1. Importe le dataset pokemon.csv. Chaque ligne représente un pokemon, avec ses différentes caractéristiques (attaque, défense, vitesse, etc...), ainsi que la colonne "légendaire".
2. Entraine l'algorithme NN en utilisant l'ensemble des colonnes numériques en variables explicatives X.

> - Les valeurs nulles (NaN) posent problème à l'ensemble des algorithmes. Ici, pour simplifier, tu peux supprimer la colonne concernée avant d'entrainer ton modèle.
> - Pas besoin de traintestsplit dans ce cas précis : en effet, sinon tu chercheras les voisins sur un sous-échantillon. Alors qu'il y a peut-être des voisins plus proche.
> - Pas besoin de predict ou de score non plus : nous calculons uniquement des distances.

3. Utilise la fonction kneighbors() pour trouver le ou les Pokémons le(s) plus proche(s) de chacun des Pokémon légendaires que le champion a l'habitude d'utiliser.
4. Fais des recommandations de Pokémon à utiliser par le champion pour sa prochaine compétition, en lui priorisant par distance. Evidemment, ta recommandation ne doit pas indiquer un autre pokemon légendaire, même si ce dernier est très proche...

## Critères de validation
- Les solutions sont dans un notebook et peuvent être lues par toute personne ayant le lien.
- Il y a une liste de recommandations de Pokémon.
- La recommandation est basée sur l'utilisation de k-NN.

