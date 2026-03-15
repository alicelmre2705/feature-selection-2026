# Towards an Interpretable Fuzzy Approach to Experimental Design

## Feature Selection for Fuzzy Clustering — Comparative Benchmark

**Auteur : Alice Lemaire**
CentraleSupelec — Pole Projet IA & ML | En collaboration avec le CEA-LIST

---

## Contexte

Le CEA-LIST a developpe un algorithme d'aide a la decision pour l'optimisation experimentale en science des materiaux, reposant sur un **clustering flou** (Fuzzy C-Means) couple a un systeme d'inference de Sugeno. L'algorithme produit des regles interpretables, mais leur lisibilite se degrade lorsque le nombre de variables est eleve.

Ce projet realise un **benchmark comparatif de 9 methodes de selection de variables** appliquees en amont de 3 algorithmes de clustering flou, sur 10 jeux de donnees (4 materiaux, 6 real-world UCI) — soit **270 experiences** au total.

L'objectif est d'identifier les methodes de selection les plus adaptees pour reduire la dimensionnalite tout en preservant la qualite du clustering et l'interpretabilite des regles.

## Contenu du repository

| Fichier / Dossier | Description |
|---|---|
| `01_Presentation.pdf` | Presentation du projet (CentraleSupelec / CEA-LIST) |
| `02_CEA_Algorithme_Flou_EN.pdf` | Article de reference : *Towards an Interpretable Fuzzy Approach to Experimental Design* (Rousselle, Poli & Ben Abdallah, 2024) |
| `CEA_LIST_Benchmark_FINAL_1.ipynb` | Notebook Python du benchmark complet |
| `CEA_LIST_Benchmark_FINAL_1.pdf` | Export PDF du notebook |
| `figures/` | 7 figures de synthese (heatmaps, classements, compromis) |
| `Datasets/` | 10 jeux de donnees CSV + descriptions TXT |

## Methodes de selection comparees

- Variance Threshold
- Correlation Filter
- Mutual Information
- Laplacian Score
- PCA (composantes principales)
- Random Forest Importance
- LASSO (L1)
- Recursive Feature Elimination (RFE)
- Boruta

## Algorithmes de clustering

- Fuzzy C-Means (FCM)
- Gustafson-Kessel (GK)
- Fuzzy K-Medoids

## Reference

> C. Rousselle, J.-P. Poli & L. Ben Abdallah, *Towards an Interpretable Fuzzy Approach to Experimental Design*, 2024.

## Correspondants CEA-LIST

- Camille Fouillard
- Raphael Belloum

## Licence

Projet academique — CentraleSupelec / CEA-LIST.
