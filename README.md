# Results

(English below)

Ce répertoire contient les différents résultats de l'analyse distributionnelle présentée dans l'étude : 
* les scores de proximité des amorces ("seeds" en anglais) entre elles (average_proximity_seeds.txt)
* les voisins distributionnels des barycentres de chaque suffixe (list_neighbors_\*.csv)

Les scores de proximité des amorces entre elles sont présentés dans un fichier .csv composé de 3 colonnes séparées par des tabulations. Le fichier présente l'ensemble des amorces (tout suffixe confondu). Chaque entrée comprend :
* le suffixe du nom d'agent
* le nom d'agent
* le score de proximité moyen (sur 5 modèles) du nom d'agent à l'ensemble des autres noms d'agent construits par le même procédé
Ainsi, le score de proximité associé à *agonisant* dans ce fichier correspond au score de proximité moyen de *agonisant* à l'ensemble des autres noms en -*ant* de la liste (*appelant, apprenant, arrivant*, etc), moyenné sur 5 modèles.

Les voisins distributionnels sont présentés dans des fichiers .csv (un par suffixe) composés de 7 colonnes séparées par des tabulations. Chaque entrée contient :
* le voisin distributionnel avec le POS annoté par le parseur (NEIGHBOR)
* le barycentre duquel il est voisin (CENTROID)
* son score cosinus de proximité au barycentre (compris entre 0 et 1, dec = .)
* son type morphologique (MORPH_TYPE, parmi "affixed", "conversion", "compound", "complex", "simple", "extragram" et "undet")
* son suffixe ou préfixe lorsque c'est pertinent (EXPONENT)
* la catégorie grammaticale de sa base lorsque c'est pertinent (BASE_POS, parmi "v", "n" et "a")
* le type sémantique de sa base lorsque c'est pertinent (SEM_TYPE, parmi "action", "object", "domain", "property", "institution", "objCog" et "other")

## English version

This repository contains the various resuls from the distributional analysis of the study :
* the proximity scores of seeds ("amorces" in the paper) with each others (average_proximity_seeds.txt)
* the distributional neighbors of each suffix centroid (list_neighbors_\*.csv)

The proximity scores of seeds with each others are presented in a .csv file composed of 3 columns separated by tabulations. The file contains all items (all suffixes together). Each entry contains:
* the exponent of the agent noun
* the agent noun
* the average proximity score (over 5 models) of the agent noun to the other agent nouns formed with the same exponent
Thus, the proximity score associated to *agonisant* in the file corresponds to the averaged proximity score of *agonisant* to all other -*ant* agent nouns of the list (*appelant, apprenant, arrivant*, etc), averaged over 5 models.

The distributional neighbors are presented in .csv files (one for each suffix) composed of 7 columns separated by tabutations. Each entry contains:
* the distributional neighbor and its POS label given by the parser (AN)
* the centroid to which it is associated (CENTROID)
* its proximity score to the centroid (between 0 and 1, dec = .)
* its morphological type (MORPH_TYPE, among "affixed", "conversion", "compound", "complex", "simple", "extragram", and "undet")
* its exponent (suffix or prefix) if relevant (EXPONENT)
* its base's part-of-speech if relevant (BASE_POS, among "v", "n" and "a")
* its base's semantic type if relevant (SEM_TYPE, among "action", "object", "domain", "property", "institution", "objCog" and "other")
