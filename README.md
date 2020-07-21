# Results

(English below)

Ce répertoire contient les différents résultats de l'analyse distributionnelle présentée dans l'étude : 
* les scores de proximité des amorces entre elles (...)
* les voisins distributionnels des barycentres de chaque suffixe (list_neighbors_\*.csv)

Les scores de proximité des amorces entre elles sont présentés dans ... (COMING SOON)

Les voisins distributionnels sont présentés dans des fichiers .csv (un par suffixe) composés de 7 colonnes séparées par des tabulations. Chaque entrée contient :
* le voisin distributionnel avec le POS annoté par le parseur (AN)
* le barycentre duquel il est voisin (CENTROID)
* son score cosinus de proximité au barycentre (compris entre 0 et 1, dec = .)
* son type morphologique (MORPH_TYPE, parmi "affixed", "conversion", "compound", "complex", "simple", "extragram" et "undet")
* son suffixe ou préfixe lorsque c'est pertinent (EXPONENT)
* la catégorie grammaticale de sa base lorsque c'est pertinent (BASE_POS, parmi "v", "n" et "a")
* le type sémantique de sa base lorsque c'est pertinent (SEM_TYPE, parmi "action", "object", "domain", "property", "institution", "objCog" et "other")



## English version

This repository contains the various resuls from the distributional analysis of the study :
* the proximity scores of seeds ("amorces" in the paper) with each others
* the distributional neighbors of each suffix centroid (list_neighbors_\*.csv)

The proximity scores of seeds with each others are presented ... (COMING SOON)

The distributional neighbors are presented in .csv files (one for each suffix) composed of 7 columns separated by tabutations. Each entry contains:
* the distributional neighbor and its POS label given by the parser (AN)
* the centroid to which it is associated (CENTROID)
* its proximity score to the centroid (between 0 and 1, dec = .)
* its morphological type (MORPH_TYPE, among "affixed", "conversion", "compound", "complex", "simple", "extragram", and "undet")
* its exponent (suffix or prefix) if relevant (EXPONENT)
* its base's part-of-speech if relevant (BASE_POS, among "v", "n" and "a")
* its base's semantic type if relevant (SEM_TYPE, among "action", "object", "domain", "property", "institution", "objCog" and "other")
