# 📊 Prévision des ventes Walmart – Projet Data Science

## 🧠 Présentation du projet
Ce projet vise à analyser et prédire les **ventes hebdomadaires des magasins Walmart** à partir de données historiques et de facteurs externes tels que les jours fériés, la température, le prix du carburant, l’inflation (CPI), le chômage et les promotions (MarkDown).

L’objectif est de construire un **modèle de machine learning capable de prédire les ventes avec précision**, afin d’aider à la prise de décision en entreprise (gestion des stocks, planification, stratégie commerciale).

---

## 🎯 Objectifs
- Réaliser une analyse exploratoire des données (EDA)
- Nettoyer et traiter les données manquantes et aberrantes
- Créer de nouvelles variables pertinentes (feature engineering)
- Encoder les variables catégorielles
- Construire et évaluer des modèles de régression
- Améliorer les performances via l’ingénierie des variables

---

## 📂 Description des données
Le dataset contient :

- **Store / Dept** : identifiants des magasins et départements  
- **Date / Week** : information temporelle  
- **Weekly_Sales** : variable cible (ventes hebdomadaires)  
- **Temperature, Fuel_Price, CPI, Unemployment** : variables économiques  
- **MarkDown1–5** : promotions et réductions  
- **IsHoliday** : indicateur de jour férié  
- **Size / Type** : caractéristiques des magasins  

---

## 🧹 Prétraitement des données
- Traitement des valeurs manquantes (MarkDown)
- Gestion des valeurs aberrantes (méthode IQR)
- Encodage des variables catégorielles (`Store`, `Dept`, `Type`)
- Standardisation des variables numériques
- Transformation logarithmique de `Weekly_Sales`
- Création de variables de retard (`Lag_1` à `Lag_4`)
- Création d’une variable indicatrice de promotions (Flag MarkDown)

---

## 🧪 Feature Engineering
- 📆 Variables temporelles (année, semaine, saisonnalité)
- 🎯 Indicateur de promotion (MarkDown Flag)
- 📉 Variables de retard (Lag features)

---

## 🤖 Modèles utilisés
- Linear Regressor  
- Random Forest Regressor  
- XGBoost Regressor

---

## 📊 Évaluation du modèle
Les métriques utilisées :
- MAE (Erreur absolue moyenne)
- MSE (Erreur quadratique moyenne)
- RMSE (Racine de l'Erreur Quadratique Moyenne) 
- R² Score

### Résultats obtenus :
- **R² ≈ 0.96**
- **MAE ≈ 1 651**
- **RMSE ≈ 4 422**

---

## 📈 Résultats et insights
- Les ventes sont fortement asymétriques avec des pics importants
- Les promotions (MarkDown) influencent fortement les ventes
- Les périodes de fêtes ont un impact majeur
- Les variables temporelles améliorent fortement les performances
- Les variables de retard (lags) sont très utiles pour la prédiction

---

## ⚙️ Technologies utilisées
- Python  
- Pandas / NumPy  
- Scikit-learn  
- Matplotlib / Seaborn  
- Jupyter Notebook  

---

## 🚀 Améliorations futures
- Utilisation de d'autres modèles avancés (LightGBM)
- Modèles de séries temporelles (SARIMA, Prophet)
- Sélection automatique des variables importantes

---

## 📌 Conclusion
Ce projet présente un pipeline complet de data science :
**nettoyage → exploration → feature engineering → modélisation → évaluation**

Il constitue une base solide pour la prévision des ventes dans le secteur retail.

---

## 👤 Participants
- Roslin Ivan Jouanang Komguep (Auteur)
- Kendric Guerrin Tatchuenwa Nziguem (Contributeur)
- Aissata Sanoh (Contributeur)
- Wilson Dongmo Nentedemo (Contributeur)
