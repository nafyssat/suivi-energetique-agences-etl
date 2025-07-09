# Suivi énergétique d’un réseau d’agences  
**Pipeline ETL avec Talend, PostgreSQL et Metabase**

## Contexte

Les entreprises multi-sites (banques, commerces, logistique) cherchent à mieux maîtriser leur consommation électrique.  
Cependant, elles disposent rarement de systèmes centralisés permettant de suivre et exploiter ces données efficacement.

## Problématique

Comment regrouper, nettoyer et structurer des données de consommation électrique provenant de sites distants, afin de :

- Identifier les bâtiments les plus énergivores
- Comparer les performances entre agences
- Mettre en place des indicateurs de suivi fiables

## Objectif

Mettre en place un pipeline ETL complet permettant de :

1. Extraire des données open source sur la consommation électrique d’entreprises
2. Filtrer et transformer les données pour simuler un parc d’agences
3. Charger les données dans PostgreSQL
4. Construire un tableau de bord avec Metabase

## Données utilisées

- **Source :** Enedis Open Data  
- **Dataset :** Consommation annuelle des entreprises par adresse  
- **Lien :** https://data.enedis.fr/explore/dataset/consommation-annuelle-entreprise-par-adresse/  
- **Contenu :** adresse, année, consommation annuelle, secteur (tertiaire, industriel, etc.)

## Outils

- Talend Open Studio : ETL graphique
- PostgreSQL : base de données relationnelle
- Metabase : visualisation des indicateurs
- Python (optionnel) : pré-traitement ou enrichissement

## Architecture

1. Ingestion du fichier CSV
2. Nettoyage et filtrage par secteur et région
3. Enrichissement (surface, type de site simulé)
4. Chargement en base PostgreSQL
5. Restitution via tableau de bord

## Portée

Ce projet est à but pédagogique.  
Il utilise des données publiques anonymisées, et simule un cas métier entreprise dans un cadre d’apprentissage.

