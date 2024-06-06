# Modèle-de-scoring
Construction d'un modèle de scoring pour aider les équipes métiers à accorder un crédit à un client.

# Contexte:
La société financière “Prêt à dépenser” souhaite développer un algorithme de scoring pour aider les chargés clientèles à attribuer ou non un crédit à un client. Pour cela, une transformation des données pertinentes pour le modèle de scoring sera faite sur le jeu de données “application_train.csv “ contenant des informations générales et financières sur le client et sur le crédit.

# Objectif:
Faire une analyse exploratoire d'un jeu de données et constuire un modèle de scoring à partir de jeu de données:

# Données
[Lien de l'adresse du jeu de données](https://github.com/CactusDeMexico/Portfolio/blob/master/Openclassrooms_IA/Projet_4/README.md#lentra%C3%AEnement-dun-mod%C3%A8le-supervis%C3%A9-classique-r%C3%A9pondant-%C3%A0-la-probl%C3%A9matique-m%C3%A9tier-est-pertinente-si-:~:text=%F0%9F%93%84%20Dataset-,olist,-%F0%9F%93%88%20Comp%C3%A9tences%20%C3%A9valu%C3%A9es)

# Plan:

#### Analyse de données et nettoyage des données - <i>Transformer les variables pertinentes pour un modèle supervisé classique (= feature engineering)
>- analyse exploratoire sur les variables initiales
>- identification et traitement des données maquantes (suppression des échantillons si peu nombreux/ prendre moyenne/ faire regression)
>- identification et traitement des outliers (prendre leur log/max)
>- normalisation des valeurs numériques (Min-Max-Scaling/ Z-score Standardisation)
>- encodage des données binaires/ catégorielles(Methode One-hot/ Encodage binaire)
>- Augmenter le dataset (transformation, construction de nouvelles varaibles à partir de celles existantes)
>- Répresentation graphique de l'importance des variable (calcul de corrélation: Pearson/ ANOVA/ calcul du CHI-2)

#### Entraînement du modèle - <i> Entraîner un modèle supervisé classique qui répond aux attentes des métiers
>- Identification de la variable cible
>- séparation du jeu de données en Train/ Test (pas de fuite d'information du jeu de test vers le jeu d'entrainement : normaliser les données uniquement sur le jeu d'entrainement puis sur celui de test)
>- Entrainement d'un modèle linéaire (regression lineaire) et calcul de la performance (score/ RSME/ MAPE)
>- Entrainement d'un modele non lineaire (regression polynomiale)
>- Mesure de l'importance des variables ( reg.coef_/ clf.feature_importances_ : pour forets aléatoires)

 #### Evaluation du modèle - <i> Evaluer les performances d’un modèle supervisé classique
 >- Calcul d'une métrique adapté pour calculer les performances des modèles
 >- Calcul de la performance d'un modèle simple pour servir de bechmarck pour le calcul de la performance de modèles plus complexes
 >- Implementer la validation croisée sur les différents modèles (GridSearchCV)
 >- Synthèse comparative des différents modèles (classification_rapport/ matrice de confusion)
 >-  Explication du choix de la métrique d'évalutation
 >-  Hyperparametres optimisés (max_depth, learning_rate, n_estimators : RandomForest/ GradientBoosting) avec GridSearch / Validation croisée

 #### Librairies Python:
 >- Pandas
 >- Matplotlib
> - Spicy
> - Sklearn
> - Seaborn
> - Numpy 
















 
