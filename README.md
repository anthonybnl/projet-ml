# Projet Machine Learning

## Contexte

L’obésité constitue aujourd’hui un enjeu majeur de santé publique à l’échelle mondiale. Elle est associée à de nombreux risques médicaux tels que les maladies cardiovasculaires, le diabète ou encore certains troubles métaboliques. La progression de l’obésité dans la population s’explique notamment par des facteurs liés au mode de vie, aux habitudes alimentaires, à l’activité physique ou encore à des prédispositions familiales.

Avec la disponibilité croissante de données individuelles relatives aux comportements alimentaires et au mode de vie, les méthodes de machine learning offrent de nouvelles possibilités pour analyser ces facteurs et identifier des profils à risque. L’exploitation de ces données permet ainsi de mieux comprendre les déterminants de l’obésité et d’anticiper l’évolution de l’état de santé des individus.

## Objectif métier

L’objectif de ce projet est de développer un modèle de classification capable de prédire le niveau d’obésité d’un individu à partir de caractéristiques démographiques, physiques et comportementales. Ce type de modèle peut permettre à des acteurs du secteur de la santé, des assurances ou des applications de suivi nutritionnel d’identifier plus facilement les personnes présentant un risque accru d’obésité.

Une telle approche peut contribuer à mettre en place des actions de prévention ciblées, proposer des recommandations personnalisées en matière de nutrition et d’activité physique, et plus largement soutenir les initiatives visant à améliorer la santé publique et à réduire les coûts associés aux maladies liées à l’obésité.

## Description du dataset

Source des données : [Kaggle - Obesity Prediction Dataset](https://www.kaggle.com/datasets/adeniranstephen/obesity-prediction-dataset)

Le jeu de données utilisé dans ce projet provient de la plateforme Kaggle et porte sur la prédiction du niveau d’obésité à partir d’informations liées au mode de vie et aux caractéristiques physiques des individus. Il contient des observations décrivant différents facteurs susceptibles d’influencer le poids et l’état de santé, tels que les habitudes alimentaires, l’activité physique ou encore certaines caractéristiques démographiques.

Le dataset comporte 17 variables, dont 16 variables explicatives et 1 variable cible. Ces variables incluent à la fois des données numériques (âge, taille, poids, fréquence d’activité physique, etc.) et des données catégorielles (genre, habitudes alimentaires, consommation d’alcool, moyen de transport, etc.).

La variable cible du modèle est NObeyesdad, qui représente le niveau d’obésité de l’individu. Cette variable est une variable catégorielle composée de sept classes correspondant à différents niveaux de poids :

- Insufficient Weight
- Normal Weight
- Overweight Level I
- Overweight Level II
- Obesity Type I
- Obesity Type II
- Obesity Type III

Détail des colonnes :

- Gender – Male or Female.
- Age – The person’s age in years.
- Height – Height in meters.
- Weight – Weight in kilograms.
- family_history_with_overweight – Whether the person has a family history of being overweight (yes/no).
- FAVC – If the person frequently consumes high-calorie foods (yes/no).
- FCVC – Frequency of vegetable consumption (scale from 1 to 3).
- NCP – Number of main meals per day.
- CAEC – Frequency of consuming food between meals (Never, Sometimes, Frequently, Always).
- SMOKE – Whether the person smokes (yes/no).
- CH2O – Daily water intake (scale from 1 to 3).
- SCC – If the person monitors their calorie intake (yes/no).
- FAF – Physical activity frequency (scale from 0 to 3).
- TUE – Time spent using technology (scale from 0 to 3).
- CALC – Frequency of alcohol consumption (Never, Sometimes, Frequently, Always).
- MTRANS – Main mode of transportation (Automobile, Bike, Motorbike, Public Transportation, Walking).
- NObeyesdad – Obesity level (Insufficient Weight, Normal Weight, Overweight Level I, Overweight Level II, Obesity Type I, Obesity Type II, Obesity Type III).

## Méthodologie

Pour atteindre l’objectif de prédiction du niveau d’obésité, nous avons suivi une méthodologie structurée en plusieurs étapes clés :

- EDA (Exploratory Data Analysis)
- Prétraitement des données (Data Cleaning, Feature Engineering)
- Application d'un modèle non supervisé (PCA) pour la réduction de dimensionnalité
- Application de modèles supervisés (Random Forest, Gradient Boosting, Logistic Regression)
- Évaluation des performances des modèles
- Interprétation des résultats et recommandations

Voir le notebook [Obesity_Prediction.ipynb](./Obesity_Prediction.ipynb) pour les détails de l’implémentation et les résultats obtenus.
