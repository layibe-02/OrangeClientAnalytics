# Orange Summer Challenge

##  Analyse des Clients Orange

**Nom :** LAYIBE YAYIBE  
**Prénom :** Narcisse

---

##  Librairies utilisées

- `pandas` : Manipulation et analyse de données tabulaires  
- `numpy` : Calculs numériques  
- `matplotlib` / `seaborn` : Visualisation de données  
- `scikit-learn` : Modélisation prédictive, machine learning  

---

## Résumé des observations

| Cluster | Âge moyen | Data (Mo) | Appels (min) | SMS envoyés | Montant facture | Forfait |
|--------:|-----------:|-----------:|--------------:|-------------:|-----------------:|---------:|
| 0       | 56.5       | 1706.5     | 183.0         | 28.8         | 5235.8           | Postpayé (1) |
| 1       | 29.8       | 1567.8     | 217.7         | 27.0         | 5376.4           | Postpayé (1) |
| 2       | 43.7       | 1582.9     | 201.3         | 29.6         | 4974.9           | Prépayé (0) |
| 3       | 44.2       | 1096.0     | 227.5         | 34.7         | 4643.5           | Principalement Postpayé (≈1) |

**Analyse rapide :**
- Le **cluster 2** est composé d’utilisateurs en **prépayé** avec une **forte consommation**, ce qui en fait une **cible idéale pour une migration vers un forfait postpayé**.
- Le **cluster 0** représente des **utilisateurs plus âgés** avec une consommation importante, idéal pour des offres de fidélisation.
- Le **cluster 1** est jeune et très connecté, idéal pour des campagnes numériques et des offres combinées.
- Le **cluster 3** est orienté **voix/SMS**, intéressant pour des offres traditionnelles ou hybrides.

---

## Recommandations business

| Objectif                              | Action Recommandée                                              |
|--------------------------------------|------------------------------------------------------------------|
| Augmenter ARPU                       | Upsell vers forfaits supérieurs (clusters 0 et 1)                |
| Convertir prépayés à haut potentiel  | Migration cluster 2 vers postpayé avec bonus                     |
| Réduire churn                        | Fidélisation clients postpayés par avantages exclusifs           |
| Cibler jeunes sur digital            | Campagnes réseaux sociaux (cluster 1)                            |
| Valoriser usage voix/SMS            | Packs d’appels/SMS ciblés, offres mixtes pour cluster 3          |

---

## Recommandations par cluster

### Cluster 0 : Seniors connectés
- Bonus data ou options premium (YouTube, WhatsApp illimité)
- Upsell vers forfaits supérieurs
- Programme de fidélité et service client renforcé

### Cluster 1 : Jeunes très connectés
- Offres combinées (data + musique/streaming)
- Parrainage, campagnes réseaux sociaux
- Gamification des offres

### Cluster 2 : Prépayé à fort potentiel
- Campagnes de migration vers postpayé
- Bonus à l’activation d’un forfait
- Simulation d’économies réalisées via migration

### Cluster 3 : Fort usage voix/SMS
- Packs d’appels illimités et bonus SMS
- Migration vers offres mixtes (voix + data)
- Offres VoIP incluses

---

## Ce qui aurait pu être ajouté avec plus de temps

- Visualisation des clusters en 2D (t-SNE)
- Segmentation plus fine avec d’autres variables (ex : fréquence de recharge, satisfaction client)
- Intégration des données temporelles pour suivre l’évolution des comportements
- Validation de la stabilité des clusters avec silhouette score ou Davies-Bouldin

---
