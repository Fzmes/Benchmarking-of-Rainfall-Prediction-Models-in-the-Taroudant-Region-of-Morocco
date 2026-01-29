# 🌧️ Benchmarking de Modèles de Prédiction des Précipitations - Région de Taroudant (Maroc)

*Comparaison de modèles ML/DL optimisés utilisant des données NASA/POWER NWP (2000-2025)*

---

## 📋 Tableau des Stratégies d'Optimisation par Modèle

| Modèle | Stratégie d'Optimisation Principale |
|--------|--------------------------------------|
| **XGBoost** | Pondération adaptative des pics (3-13×) + ingénierie de features avancée (48+ features météo et temporelles) |
| **Random Forest** | Échantillonnage équilibré focalisé sur les pics + dataset réduit mais optimisé |
| **LSTM** | Modélisation séquentielle automatique + capture des dépendances temporelles via fenêtres glissantes |

---

## 🎯 Objectif du Projet

Ce projet effectue un **benchmarking rigoureux** de trois familles de modèles pour la **prédiction des pics de précipitations** dans la **région de Taroudant au Maroc**, en utilisant des **données NASA POWER (NWP) de 2000 à 2025**.

Chaque modèle a été **spécifiquement optimisé** pour capturer les dynamiques complexes des précipitations en climat semi-aride, avec un focus particulier sur la **détection des événements extrêmes**.

---

## 📊 Résultats des Modèles Optimisés

| Modèle | MAE (mm) | RMSE (mm) |
|--------|----------|-----------|
| **XGBoost** | **0.0027** | **0.0588** |
| **Random Forest** | 0.0038 | 0.0720 |
| **LSTM** | 0.0254 | 0.2110 |

---

## 🔍 Conclusions Clés

1. **XGBoost excelle** grâce à sa combinaison de pondération intelligente et d'ingénierie de features riche
2. **Random Forest offre** le meilleur équilibre performance/interprétabilité
3. **LSTM capture** bien les tendances mais sous-performe sur les pics isolés
4. Les **approches hybrides** (features temporelles + pondération adaptative) surpassent les modèles purs

---

## 🛠️ Architecture Technique

```
Données NASA POWER (2000-2025)
         ↓
Prétraitement & Feature Engineering
         ↓
Optimisation spécifique par modèle
         ↓
Évaluation multi-métriques
         ↓
Visualisation comparative
```

---

## 💡 Pourquoi Ce Projet est Pertinent

- ✅ **Problématique réelle** : Prédiction des risques d'inondation en zone semi-aride
- ✅ **Données opérationnelles** : NASA POWER largement utilisé en climatologie
- ✅ **Approche professionnelle** : Chaque modèle poussé dans ses limites d'optimisation
- ✅ **Analyse nuancée** : Métriques globales ET spécifiques aux événements extrêmes

---

## 📈 Perspectives d'Amélioration

1. **Ensemble learning** : Combinaison des trois modèles
2. **Transfer learning** : Application à d'autres régions climatiques
3. **Prévisions probabilistes** : Intervalles de confiance
4. **Intégration en temps réel** : API de prédiction opérationnelle

---

## 📄 Licence

**Données NASA POWER** : Libre accès  
**Code** : Apache 2.0 License  

⚠️ **À noter** : Les performances sont spécifiques à la région de Taroudant et peuvent varier selon la zone climatique.

---

## 📧 Contact

**Équipe** : Fatima Ezzahra Meskine • Najlae Babadaih • Ikram Ait Ben Mbark  

**Date** : 2025

Pour toute question, collaboration ou demande d'accès aux données :

- 📧 Email : meskinefatimaezzahra@gmail.com
- 🌐 LinkedIn : [[LinkedIn](https://www.linkedin.com/in/fatima-ezzahra-meskine/)]
- 🐦 Twitter : 

**Domaine** : Climatologie Appliquée & Data Science

---

*Projet développé dans le cadre de l'amélioration des systèmes d'alerte précoce pour les événements climatiques extrêmes au Maroc*
