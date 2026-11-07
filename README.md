# Customer Churn Prediction

## 1. Présentation du projet

Ce projet consiste à analyser et prédire le désabonnement des clients (*Customer Churn*) d'une entreprise de télécommunications à l'aide de techniques de Machine Learning.

L'objectif est d'identifier les clients susceptibles de résilier leur abonnement afin d'aider l'entreprise à améliorer ses stratégies de fidélisation.

## 2. Objectifs

- Analyser les données des clients.
- Identifier les facteurs associés au désabonnement.
- Construire des modèles de classification.
- Comparer les performances des modèles.
- Identifier les clients présentant un risque de résiliation.

## 3. Technologies utilisées

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab

## 4. Méthodologie

1. Data Cleaning et préparation des données.
2. Exploratory Data Analysis (EDA).
3. Encodage des variables catégorielles.
4. Séparation des données en ensembles d'entraînement et de test.
5. Feature Scaling.
6. Entraînement des modèles :
   - Logistic Regression
   - Random Forest
7. Évaluation et comparaison des modèles.
8. Analyse de l'importance des variables (*Feature Importance*).

## 5. Résultats

| Modèle | Accuracy | Recall (Churn = 1) |
|---|---:|---:|
| Logistic Regression | 80.38% | 57% |
| Logistic Regression Balanced | 72.99% | 80% |
| Random Forest Balanced | 78.68% | 49% |

Le modèle Logistic Regression avec `class_weight='balanced'` a obtenu le meilleur Recall (80%).

Il a donc été retenu comme modèle privilégié pour détecter le maximum de clients susceptibles de résilier leur abonnement.

## 6. Feature Importance

Les variables les plus importantes identifiées par Random Forest sont :

- TotalCharges
- tenure
- MonthlyCharges
- Contract_Two year
- PaymentMethod_Electronic check

## 7. Conclusion

Ce projet m'a permis de mettre en pratique les principales étapes d'un projet de Machine Learning, depuis la préparation des données jusqu'à l'évaluation des modèles.

Il m'a également permis de comprendre l'importance du choix des métriques d'évaluation, notamment le Recall et la Precision.

**Perspective :** améliorer les performances des modèles et développer des stratégies de fidélisation adaptées aux clients à risque.
