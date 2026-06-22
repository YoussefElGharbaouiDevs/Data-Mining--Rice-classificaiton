# Projet de Classification de Variétés de Riz

Ce projet a pour objectif de développer un modèle de machine learning capable de distinguer deux variétés de riz, Cammeo et Osmancik, en se basant sur des caractéristiques morphologiques extraites d'images.

## Problématique

L'enjeu est de déterminer si une classification automatique et fiable est possible à partir de 7 mesures morphologiques, afin d'automatiser le tri des grains de riz, une tâche traditionnellement manuelle, coûteuse et sujette aux erreurs.

## Dataset

Le jeu de données utilisé est le **"Rice (Cammeo and Osmancik)"** de l'UCI Machine Learning Repository.

- **Source :** [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/545/rice+cammeo+and+osmancik)
- **Caractéristiques :** 7 variables numériques (Area, Perimeter, Major_Axis_Length, etc.).
- **Cible :** 1 variable catégorielle binaire (`CLASS`) indiquant la variété (Cammeo ou Osmancik).

## Démarche

Le notebook `Projet2_Classification_Riz.ipynb` détaille les étapes suivantes :
1.  **Importation des bibliothèques** (Pandas, Scikit-learn, Matplotlib, Seaborn).
2.  **Chargement et exploration des données** pour comprendre leur structure.
3.  **Analyse exploratoire des données (EDA)** avec des visualisations pour identifier les relations entre les variables.
4.  **Prétraitement des données**, incluant la séparation des ensembles d'entraînement et de test et la standardisation des features.
5.  **Modélisation** avec plusieurs algorithmes de classification :
    - Régression Logistique
    - K-Nearest Neighbors (KNN)
    - Support Vector Machine (LinearSVC)
    - Random Forest
6.  **Évaluation des modèles** à l'aide de métriques comme l'accuracy, precision, recall, le F1-score et les matrices de confusion.

## Résultats

Le projet démontre qu'il est possible d'atteindre une excellente performance de classification, avec des modèles comme le Random Forest obtenant une accuracy très élevée, validant ainsi l'approche d'automatisation du tri.

## Comment utiliser

1.  Clonez le dépôt.
2.  Installez les dépendances : `pip install -r requirements.txt`
3.  Ouvrez et exécutez le notebook `Projet2_Classification_Riz.ipynb` dans un environnement Jupyter.

