# Projet d'Analyse des Données de Football

## Description du Projet
Ce projet vise à analyser des données de football, notamment les performances des joueurs, les résultats des équipes, et les tendances des matchs, à travers des techniques de data science et de visualisation. Les objectifs principaux sont :
- Identifier les meilleurs joueurs, équipes, et matchs à haut score.
- Regrouper (clustering) les joueurs et les équipes en fonction de leurs caractéristiques.
- Visualiser les tendances temporelles et interpréter les résultats pour des recommandations stratégiques.

---

## Étapes du Projet
### **1. Préparation des Données**
- Chargement des fichiers suivants :
  - `players_df`: Données des joueurs contenant leurs caractéristiques et performances.
  - `matches_df`: Données des matchs avec les résultats et détails des équipes.
  - `teams_df`: Attributs des équipes liés à leurs styles de jeu.
- Nettoyage des données :
  - Suppression des valeurs manquantes.
  - Ajout de colonnes calculées comme `performance_metric` et `total_goals`.

### **2. Analyse des Joueurs**
- Calcul de la métrique de performance basée sur :
  - **Évaluation globale (`overall_rating`)**
  - **Potentiel (`potential`)**
  - **Passes courtes (`short_passing`)**
  - **Tacles debout (`standing_tackle`)**
- Identification des meilleurs joueurs.

### **3. Analyse des Équipes**
- Calcul des victoires à domicile et à l'extérieur pour identifier les équipes dominantes.
- Analyse des styles de jeu des équipes.

### **4. Analyse des Matchs**
- Identification des matchs avec le plus grand nombre de buts.
- Analyse des performances à domicile vs extérieur.

### **5. Clustering**
- **Clustering des joueurs** :
  - Basé sur les attributs comme `overall_rating`, `potential`, `height`, et `weight`.
- **Clustering des équipes** :
  - Basé sur les attributs comme `buildUpPlaySpeed`, `buildUpPlayPassing`, et `chanceCreationPassing`.

### **6. Présentation des Résultats**
#### **Tableaux de Résumé**
- Meilleurs joueurs.
- Équipes dominantes.
- Matchs à haut score.

#### **Graphiques et Visualisations**
- Diagrammes pour les performances des équipes.
- Scatter plots pour les clusters de joueurs et d’équipes.
- Courbes temporelles des tendances.

#### **Interprétations Clés**
- Analyse des résultats obtenus.
- Recommandations stratégiques pour maximiser les performances.

---

## Résultats Attendues
- Classements des joueurs, équipes et matchs.
- Groupes (clusters) identifiant les caractéristiques similaires des joueurs et des équipes.
- Tendances temporelles illustrant l'évolution des performances.

---

## Prérequis
### Fichiers de Données
Assurez-vous que les fichiers suivants sont disponibles dans le répertoire du projet :
1. `players_df.csv`
2. `matches_df.csv`
3. `teams_df.csv`

### Environnements et Bibliothèques Python
Installez les bibliothèques suivantes avant d'exécuter le projet :
```bash
pip install pandas numpy matplotlib plotly scikit-learn

