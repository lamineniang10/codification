# Titre du projet
Codification géographique des communes du Sénégal pour l'intégration dans un système d'aide à la décison territoriale.
## Contexte
Le projet vise à attribuer un code unique à chaque commune du Sénégal (hors communes de ville : Dakar, Pikine, Guédiawaye, Rufisque Keur Massar et Thiès). Cette codification facilite la gestion, l’analyse, la cartographie et l’intégration des communes dans les systèmes d’information.
## Objectifs
* Standardiser l’identification des communes.
* Faciliter les croisements avec des données spatiales.
* Créer une base exploitable pour des projets de cartographie, de gouvernance ou de développement territorial.
## Principe de la codification
La codification vise à attribuer un identifiant unique à chaque des communes du Sénégal, à l'exception des communes de ville(Dakar, Pikine, Guédiawaye, Rufisque Keur Massar et Thies), qui ne sont pas concernées par ce système. Le principe repose sur une hiérarchie administrative, où chaque niveau hérite du code du niveau supérieur. Chaque niveau est représenté par un ou plusieurs caractères numériques, et l'ensemble du code est précédé du préfixe **"SN"**. La structure du code est la suivante:
* **Deux** caractères pour la région
* **un** caractère pour le département
* **un** caractère pour l'arrondissement
* **un** caratère pour la commune

Les codes des régions et des département sont attribués en fonction de leur ordre de création administratif, assurant une logique historique et cohérante dans l'identifiant.

Cas particuliers : Les communes chef-lieu de département et les communes non rattachées à un arrondissement, dans ces cas, la composante "arrondissement" du code est fixée à 0, indiquant l'absence d'un niveau intermédiare.

Example

`SN01532`: Commune 2 de l'arrondissement 3 du département 5 de la région 01.

`SN11202`: Commune 2 de l'arrondissement 0 du département 2 de la région 11.

Ainsi, chaque commune reçoit un identifiant unique, normé et traçable

## Bibliothèques utilisées
Les bibliothèques utlisées incluent **python3**,  **pandas** pour le traitement des données tabulaires, **geopandas** pour la manipulation des données géospatiales et **folium** pour la visualisation des communes sur une carte interactive basée sur `OpenStreetMap`
.

## Contributions
Les contributions sont les bienvenues pour améliorer la codification, signaler des erreurs ou proposer des extensions.
## Contact
Email: sidiniang20@gmail.com

