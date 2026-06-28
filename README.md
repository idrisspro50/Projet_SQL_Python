![SQL](https://img.shields.io/badge/SQL-00758F?style=for-the-badge&logo=mysql&logoColor=white) 
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) 
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white) 
![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=for-the-badge&logo=duckdb&logoColor=black) 
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge) 
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge) 

## Analyse des Entreprises à Forte Croissance 

## Présentation 

Ce projet met en œuvre une analyse de données combinant **SQL** et **Python**. 

L'objectif est d'exploiter plusieurs jeux de données représentant des **entreprises à forte croissance (Unicorn Companies)** afin d'aider un cabinet d'investissement à mieux comprendre les tendances du marché et à répondre à des questions telles que : 

- Quels sont les secteurs les plus valorisés ? 
- Quels pays concentrent le plus d'entreprises ? 
- Quels investisseurs financent le plus de licornes ? 
- Quelles sont les entreprises les mieux valorisées ? 
- Quels sont les leaders de chaque secteur ? 
- Comment évoluent les valorisations selon les secteurs ? 

--- 

## Jeu de données 

Le projet repose sur **4 fichiers CSV**. 

| Table | Description |
|--------|-------------|
| **Companies** | Informations générales (nom, ville, pays, continent) |
| **Dates** | Année de création et date d'entrée dans le statut de licorne |
| **Funding** | Valorisation, financement et investisseurs |
| **Industries** | Secteur d'activité |

--- 
## Technologies et librairies utilisés 

- SQL 
- Python 
- Pandas 
- DuckDB 
- Matplotlib 
- Seaborn 
- VS Code 
- Jupyter Notebook 

--- 

## Importation des données 

Les fichiers CSV sont chargés avec **Pandas**, puis enregistrés dans **DuckDB** afin d'exécuter des requêtes SQL directement sur les DataFrames. 

--- 

## Nettoyage des données (Python) 

- Détection des valeurs nulles (**isna**). 
- Traitement des valeurs manquantes (**fillna**). 
- Détection et suppression des doublons (**duplicated**). 

--- 

## Exploration des données 

Analyse exploratoire comprenant : 

- Statistiques descriptives. 
- Répartition géographique des entreprises. 
- Répartition des secteurs d'activité. 
- Analyse des principaux investisseurs. 

--- 

## Analyses métier (SQL) 

Les analyses sont réalisées principalement en **SQL** afin de répondre à différentes problématiques métier, comme : 

#### Top 10 Secteurs les plus valorisés 

Calcul de : 
- Valorisation moyenne. 
- Valorisation totale. 
- Nombre d'entreprises par secteur.

<img width="392" height="387" alt="image" src="https://github.com/user-attachments/assets/5c45695e-ccbf-4aae-9dfd-1ddc52b5062d" />

--- 

#### Top 10 des entreprises 

Classement des entreprises selon leur valorisation. 

<img width="533" height="382" alt="image" src="https://github.com/user-attachments/assets/f3a74fcf-4096-4484-aa49-ccc8eeb43afe" />
  
--- 

#### Classement des 3 meilleurs compagnies par secteur 

Utilisation des **Window Functions** (`DENSE_RANK`) afin d'identifier les entreprises les mieux valorisées dans chaque secteur. 
<img width="408" height="592" alt="image" src="https://github.com/user-attachments/assets/5bcbe680-6297-48ff-9889-9a434dbe1751" />

--- 

## Visualisations (Python) 

Les résultats des requêtes SQL sont ensuite visualisés avec **Matplotlib** et **Seaborn** afin de produire des graphiques facilitant l'analyse et l'interprétation des données. 

#### Top 10 Secteurs les plus valorisés 
<img width="848" height="816" alt="image" src="https://github.com/user-attachments/assets/50e0b9aa-1cc7-4c8e-b078-4792cf2d4183" />
  
#### Top 10 des entreprises

<img width="1015" height="761" alt="image" src="https://github.com/user-attachments/assets/2ab05639-11fc-4390-893f-7442a8cbd93e" />

#### Classement des 3 meilleurs compagnies par secteur

<img width="1320" height="906" alt="image" src="https://github.com/user-attachments/assets/a992d04f-2b97-45f4-abc1-8a1f612c69c4" />

--- 

## Auteur 

**Idriss FEKARI** 
