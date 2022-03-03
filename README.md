# TP Dictionnaire - Ynov Python B1

### Tips   

:raising_hand: Si vous avez des soucis n'hésitez pas à m'appeler. 
 
## Exercice 1 : Simple Dictionary 
 
 Dans un programme python créer un dictionnaire concernant les différents modèles de voiture suivant : 
 
 ```python
 
 cars = {
  "marque": "Ford",
  "modele": "Mustang",
  "annee": 1964
}

```
Avec ce dictionnaire il faudra : 

- Afficher l'année de création de la voiture
- Rajouter un attribut à la voiture : 
  - `"couleur" : "rouge"`
- Vérifier que la voiture soit bien **rouge** 
- Afficher à l'aide d'une boucle toutes les caractéristiques de la voiture
- Modifier la couleur en `bleu`
- Supprimer la clef `couleur`
 
## Exercice 2: Nested Dictionary
 
Dans cet exerice il faut modifier le dictionaire présent dans le fichier exerice2.py selon les affirmations suivantes : 
- Patrick a quitté l'entreprise cette année, nous devons donc l'enlever du dictionnaire.
- Julie a fêté son anniversaire hier, il faut donc changer son âge (elle a maintenant 26 ans).
- Paul quant à lui fêtera son anniversaire la semaine prochaine. Nous voulons donc récupérer son âge pour savoir quel âge il aura.
- Renault a rejoint l'entreprise, il faut donc le rajouter dans le dictionnaire : 
  - id : 04
  - prénom : Renault
  - nom : Dupond
  - age : 18
  

 
## Exercice 3 : Dict parsing

- Calculer la moyenne d'age des employées de la societée
- Trouver qui est l'employé le plus agé
- Vérifier que Patrick ne fait plus partie de l'entreprise

## Exerice 4 : Pandas Dictionnary - Analyse des durées de film Netflix

Dans cet exercice il va falloir utiliser les dictionnaires ainsi que la librairie `pandas`.
Nous allons manipuler les données pour pouvoir les analyser par la suite. 
Pour le moment nous partons d'un jeu de données que nous allons créer nous même pour faciliter le travail.

Pour commencer il faut créer un set de données.

```
years = [2011, 2012, 2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020]
durations = [103, 101, 99, 100, 100, 95, 95, 96, 93, 90]
```

A partir de ce **dataset** il faut : 

- Créer un dictionnaire
  - Clef : years , durations
  - Valeurs : [2011, 2012, 2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020] , [103, 101, 99, 100, 100, 95, 95, 96, 93, 90]

- Transformer ce dictionnaire en **dataframe**
  - `import pandas as pd`
  - `durations_df = pd.DataFrame(my_dict)`

- Créer une représentation graphique de votre Dataframe
  - `import matplotlib.pyplot as plt`

**Astuce** : 
  http://www.python-simple.com/python-matplotlib/pyplot.php 
  La librairie `matplot` est la libraire la plus utilisé pour la création de graphique et autre outils de visualisation.
  Il suffit d'appeler la méthode `pyplot.plot([], [])` pour créer un graphique en lui donnant comme argument 2 listes (Ou dans notre cas un Dataframe)
  
  
## Exercice 5 : Analyse poussée d'un Dataset

Maintenant que nous avons eu un aperçu de ce que nous pouvons faire à l'aide de Python, nous allons charger le dataset complet. 

A l'aide d'une méthode qui permet de **lire** les fichiers **csv** de la librairie **pandas** : 
  - Charger le fichier `netflix_data.csv`
  - Afficher les 5 premiers rangs

Il y a beaucoup de colonnes dans ce Dataset, et nous souhaitons uniquement réaliser une analyse sur la durée des films. 

