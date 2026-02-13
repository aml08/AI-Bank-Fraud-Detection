# AI Bank Fraud Detection

![Python](https://img.shields.io/badge/Python-Data_Science-3776AB?style=for-the-badge&logo=python&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-Optimization-red?style=for-the-badge)
![ROI](https://img.shields.io/badge/Business-ROI_Analysis-green?style=for-the-badge)

## Présentation du projet
Étude complète sur la **détection de fraude bancaire** via Machine Learning.
L'objectif est de montrer la chaîne de valeur complète : du code brut à l'impact financier.

---

##  1. Exploration des données
Chargement du dataset de 284 000 transactions et premières analyses via Pandas.

![Data Code](1_data_discovery.png)

---

##  2. Analyse du déséquilibre 
Le défi majeur de ce projet est le déséquilibre extrême des classes (0.17% de fraudes). J'ai utilisé `seaborn` pour visualiser cette disparité critique.

![Imbalance Code](2_class_imbalance.png)

![Imbalance Graph](2_class_imbalance_1.png)

---

##  3. Comparaison des modèles 
J'ai développé un script pour comparer 3 algorithmes (**Random Forest, Logistic Regression, XGBoost**) sur 5 métriques clés.

![Comparison Code](3_model_comparison.png)

![Comparison Graph](3_model_comparison_1.png)

---

##  4. Optimisation avancée (GridSearchCV)
Pour maximiser la performance du modèle gagnant (XGBoost), j'ai codé une recherche par grille pour trouver les meilleurs hyperparamètres (`learning_rate`, `max_depth`, `n_estimators`).

![Optimization Params](4_optimization_code.png)

![Optimization Run](4_optimization_code_1.png)

---

##  5. Performance finale
Le modèle optimisé atteint une capacité de discrimination quasi-parfaite.

** Résultat Final (Courbe ROC) :**
L'AUC de **0.97** prouve la robustesse du modèle.
![Final ROC](5_final_results.png)

---

##  6. Impact financier (ROI)
Estimation pour une banque traitant 200 000 transactions/jour :

* **Pertes évitées (Fraudes bloquées) :** ~41.3 M€ / an.
* **Économie nette estimée :** **~37.7 Millions € par an**.
