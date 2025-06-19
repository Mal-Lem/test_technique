
# 🎧 Analyse du Succès Musical – Test Technique

## 📌 Description
Ce projet de data science explore les tendances d’écoute musicale sur Spotify. Il vise à identifier les facteurs qui influencent la popularité d’un titre ou d’un artiste en analysant des données de streaming. Le but est de comprendre les dynamiques temporelles, comportementales et artistiques à l’origine du succès musical.

## 🎯 Objectif principal
**Étudier les tendances d’écoute sur Spotify afin d’identifier les facteurs de succès musical et les dynamiques temporelles qui influencent la popularité d’un titre ou d’un artiste.**

## 📂 Sous-objectifs / Axes d’analyse

1. Étudier les **évolutions de l’écoute dans le temps** (tendance générale, saisonnalité, pics d’écoute).
2. Mesurer l’**impact de la date de sortie** sur la performance d’un morceau.
3. Analyser la **relation entre le volume d’écoute et la popularité** déclarée.
4. Identifier les **artistes les plus performants** et leur régularité dans le succès.
5. Mettre en évidence les **titres les plus populaires** du dataset.
6. Comparer les **performances selon la fréquence de publication** des morceaux.

## 🧪 Méthodologie

### 1. Data Understanding
- Chargement du fichier `100-songs-audience-report.csv`.
- Visualisation des premières lignes.
- Analyse des types de données, dimensions et métadonnées.

### 2. Data Cleaning & Preparation
- Nettoyage des colonnes avec tabulations.
- Suppression des colonnes non pertinentes (`image_url`).
- Élimination des doublons (`song_id`) et des valeurs nulles (`summaries`).
- Transformation des types (date, string format, etc.).

### 3. Structuration & Transformation
- Normalisation des noms d’artistes et titres.
- Création d’un DataFrame spécifique par artiste.
- Préparation des données pour les visualisations temporelles.

### 4.Stockage des données – Base PostgreSQL

Les données issues du fichier CSV ont été stockées dans une base de données PostgreSQL pour permettre des analyses plus poussées via SQL et assurer la persistance des données.
🔧 Détails de la base :

    SGBD : PostgreSQL

    Interface de gestion : pgAdmin 4

    Nom de la base : stream_analysis

    Table principale : songs

🚀 Étapes de création :

    Création de la base de données dans pgAdmin.

    Création de la table avec une structure correspondant aux colonnes du dataset.


## 📊 Analyse prévue

- Courbes de tendance des streams dans le temps.
- Classement des artistes par nombre de morceaux populaires.
- Comparatif de performance selon la date de sortie ou la fréquence de publication.
- Calculer la fréquence de publication pour chaque artiste.
- Comparer les performances selon la fréquence de publication.
- Identifier les artistes les plus performants et leur régularité.
- Évolution des streams dans le temps.

## 📁 Structure du projet

```
projet-musical/
│
├── data/
│   └── 100-songs-audience-report.csv
├── docs/
│   └── schema de la base de données
│
├── explore_data.ipynb        # Notebook principal d'analyse
├── README.md                 # Documentation du projet
```

## ⚙️ Comment exécuter le projet

1. **Pré-requis** :
```bash
pip install pandas jupyter
```

2. **Lancer le notebook** :
```bash
jupyter notebook
```

3. Ouvrir `explore_data.ipynb` et exécuter les cellules.

## 🛠️ Outils utilisés

- Python 3.11.3
- Jupyter Notebook
- Pandas
- CSV 
- Visualisation 
