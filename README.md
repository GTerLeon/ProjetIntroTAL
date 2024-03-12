# DEFT2013 Tâche 2 :

CHEBBAH Djamel, TER Léon

## Description de la tâche

	1 ou 2 exemples de documents (avec leur identifiant)

## Statistiques corpus

	Nombre de document de train/dev/test
	Répartition des étiquettes dans chacun des sous-ensemble
	- train.csv: 8731 entrées 
	- test.csv: 1388 entrées
	Les champs importants ici sont:
	- titre: nom de la recette
	- type : type de la recette à prédire 'Entree/Plat principal/Dessert' 

## Méthodes proposées

### Run1: baseline (méthode de référence)

	Description de la méthode:
	- Tire aléatoirement parmis les 3 types de recette autant de fois qu'il y a d'entrées dans le fichier de test. 
	- Pas d'utilité à avoir le fichier d'entraînement.

### Run2: TF-IDF

	Description de la méthode:
	- Utilisation de TF_IDF qui emploi la fréquence des mots dans un texte.

### Run3: Word2Vec

	Description de la méthode:
	- Utilisation de Word2Vec avec plongement de mots.

### Run4: Modelcamembert
	Description de la méthode:
	- 

## Résultats

| Run      | macro avg f1 Score |
| -------- | --------:|
| baseline |  12,4 |
| TF-IDF   |  80  |
| Word2Vec   |  63.8 (provisoire)| 
| Modelcamembert   |   |

### Analyse de résultats
	
	Pistes d'analyse:
	* Combien de documents ont un score de 0 ? de 0.5 ? de 1 ? (Courbe ROC)
	* Y-a-t-il des régularités dans les document bien/mal classifiés ?
	* Où est-ce que l'approche se trompe ? (matrice de confusion)
	* Si votre méthode le permet: quels sont les descripteurs les plus décisifs ?


	Regardons plus en détail la méthode avec le meilleur f1_score moyen, TF-IDF:
	
	*Inserer matrice de confusion*
	On 