# Certification blanche Data Analyst - Mégane La Rocca

Projet réalisé dans le cadre de la **certification RNCP6 Data Analyst** (avril 2026).

## Contenu du notebook

Le notebook `Megane_La_Rocca_Examen_blanc.ipynb` couvre les trois volets de la certification :

### 1. SQL (1h30)
- Requêtes sur base SQLite (biblio_F.sqlite3)
- Interprétation métier des résultats

### 2. Pandas — Exploration & Feature Engineering (3h30)
- Importation et audit du dataset Cyclistic (trajets vélos Chicago)
- Analyse des valeurs manquantes et nettoyage
- Calcul de la distance à vol d'oiseau (formule de Haversine)
- Création de variables temporelles : `day_of_week`, `month`, `day_type`, `season`
- Création de `route_type` (aller simple / aller-retour) et `ride_duration_min`
- Standardisation et export du dataset nettoyé

### 3. Machine Learning (2h)
- **Régression linéaire** : prédiction de `distance_travelled_km`
- **Régression logistique** : classification `member` vs `casual`
- Évaluation (R², RMSE, MAE, accuracy, classification report)
- Vulgarisation des algorithmes et analyse des limites (underfitting / overfitting)

### 4. Business Case (à venir)
- ONG World Vision — prévu le 21/04/2026 (8h)

## Structure du dossier

- `notebooks/` : notebook d'examen blanc
- `data/` : jeux de données
  - `df_cyclistic_clean.parquet` : dataset Cyclistic nettoyé
  - `biblio_F.sqlite3` : base SQLite pour la partie SQL
- `requirements.txt` : dépendances Python

## Installation

```bash
python -m venv .venv
.venv\Scripts\activate      # Windows
source .venv/bin/activate   # Mac/Linux
pip install -r requirements.txt
```

## Lancer le notebook

```bash
jupyter notebook notebooks/Megane_La_Rocca_Examen_blanc.ipynb
```

> ⚠️ Le fichier `df_cyclistic_clean.parquet` (180 Mo) n'est pas inclus dans le repo GitHub pour respecter les limites de taille. Il est téléchargé automatiquement lors de l'exécution du notebook (cellule 8 — `examen_blanc.ipynb`).

## Auteur

Megane La Rocca — Formation Data Analyst (Vert 11-2025)