# Towards an Interpretable Fuzzy Approach to Experimental Design

## Feature Selection for Fuzzy Clustering — Comparative Benchmark

**Auteur : Alice Lemaire**
CentraleSupélec — Pôle Projet IA & ML | En collaboration avec le CEA-LIST

---

## Contexte

Le CEA-LIST a développé un algorithme d'aide à la décision pour l'optimisation expérimentale en science des matériaux, reposant sur un **clustering flou** (Fuzzy C-Means) couplé à un système d'inférence de Sugeno. L'algorithme produit des règles interprétables, mais leur lisibilité se dégrade lorsque le nombre de variables est élevé.

Ce projet réalise un **benchmark comparatif de 8 méthodes de sélection de variables** appliquées en amont de 3 algorithmes de clustering, sur 10 jeux de données (4 matériaux, 6 real-world UCI) — soit **240 expériences** au total.

L'objectif est d'identifier les méthodes de sélection les plus adaptées pour réduire la dimensionnalité tout en préservant la qualité du clustering et l'interprétabilité des règles.

Le benchmark complet est implémenté dans le notebook **`CEA_LIST_Benchmark_FINAL_1.ipynb`**.

## Contenu du repository

| Fichier / Dossier | Description |
|---|---|
| `CEA_LIST_Benchmark_FINAL_1.ipynb` | Notebook Python du benchmark complet |
| `01_Presentation.pdf` | Présentation du projet (CentraleSupélec / CEA-LIST) |
| `02_CEA_Algorithme_Flou_EN.pdf` | Article de référence : *Towards an Interpretable Fuzzy Approach to Experimental Design* (Rousselle, Poli & Ben Abdallah, 2024) |
| `figures/` | 7 figures de synthèse (heatmaps, classements, compromis) |
| `Datasets/` | 10 jeux de données CSV + descriptions TXT |

## Méthodes de sélection comparées

- Variance Threshold
- Corrélation
- Laplacian Score
- SPEC (Spectral Feature Selection)
- Sparse K-Means
- MCFS (Multi-Cluster Feature Selection)
- FWKM (Feature Weighting K-Means)
- PCA (Analyse en Composantes Principales)

## Algorithmes de clustering

- K-Means
- Hierarchical Ward
- Fuzzy C-Means (FCM)

## Métriques d'évaluation

- Silhouette Score
- Davies-Bouldin Index
- Calinski-Harabasz Index
- ARI (Adjusted Rand Index)
- NMI (Normalized Mutual Information)

## Référence

> C. Rousselle, J.-P. Poli & L. Ben Abdallah, *Towards an Interpretable Fuzzy Approach to Experimental Design*, 2024.
