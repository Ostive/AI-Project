# Employee Turnover Analysis — HumanForYou

Projet académique de data analytics : identifier les facteurs qui expliquent le taux de turnover de 15 % d'une entreprise pharmaceutique fictive (HumanForYou, 4 000 employés) et construire un modèle prédictif d'attrition. Projet réalisé en groupe, cette version consolide l'analyse finale.

## Démarche

- **Exploration** de 5 jeux de données RH (profil employé, évaluations manager, enquête satisfaction, heures d'arrivée/départ)
- **Nettoyage** : suppression des colonnes non informatives ou sensibles (genre, statut marital) pour éviter les biais
- **Traitement des valeurs manquantes** : choix de méthode par colonne (médiane, imputation par régression selon la corrélation, suppression) selon la nature de chaque variable
- **Encodage** : `OrdinalEncoder` pour les variables ordonnées, `OneHotEncoder` pour les variables catégorielles sans ordre
- **Feature engineering** : calcul du temps de travail moyen à partir des pointages horaires
- **Modélisation** : classification de l'attrition (Random Forest, SVM)

## Stack technique

Python · Pandas · NumPy · Scikit-learn · Jupyter Notebook

## Contenu

- [`employee_turnover_analysis.ipynb`](./employee_turnover_analysis.ipynb) — notebook principal (analyse complète, du nettoyage au modèle)
- `data/` — jeux de données sources (RH, évaluations, enquête, pointages)

## Lancer le projet

```bash
pip install pandas numpy scikit-learn jupyter
jupyter notebook employee_turnover_analysis.ipynb
```
