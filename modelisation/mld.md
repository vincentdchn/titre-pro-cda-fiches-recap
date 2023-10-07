# Fiche Récapitulative : Modèle Logique de Données (MLD)

Le Modèle Logique de Données (MLD) est une étape intermédiaire entre le Modèle Conceptuel de Données (MCD) et le Modèle Physique de Données (MPD). Le MLD est une représentation concrète des données d'un système, et il est directement dérivé du MCD. Voici les principales règles pour convertir un MCD en MLD :

## Règle n°1 : Transformation des Entités en Tables

Chaque entité du MCD devient une table dans le MLD.
Les propriétés (attributs) des entités deviennent les colonnes des tables correspondantes.
Le déterminant (ou discriminant) de l'entité devient également une colonne, assortie d'une contrainte d'unicité.
La clé primaire de la table est généralement un identifiant (id) auto-généré par le système de gestion de base de données (SGBD).

## Règle n°2 : Gestion des Clés Étrangères

Si l'une des cardinalités maximales de la relation vaut 1, une clé étrangère est créée du côté de l'entité où la cardinalité vaut 1.
Cette clé étrangère fait référence à l'identifiant (clé primaire) de la table associée.
Dans le cas de cardinalités maximales de 1 des deux côtés, il peut s'agir d'une erreur de conception, et les deux entités pourraient être en réalité une seule entité.

## Règle n°3 : Gestion des Relations Plusieurs-à-Plusieurs

Si les deux cardinalités maximales sont n (indiquant une relation "plusieurs à plusieurs"), la relation devient une table à part entière dans le MLD.
Cette table est souvent appelée table de liaison, d'association, de jonction ou de correspondance.
Elle contient deux clés étrangères, chacune faisant référence aux tables d'entités liées.

## Exemple :

En utilisant l'exemple précédent du MCD, voici le MLD correspondant :

#### Tables Principales :

Auteur (CodeAuteur, Nom, Prénom)
Livre (ISBN, Titre, Année, #CodeAuteur) [avec une clé étrangère vers Auteur]
Genre (CodeGenre, Nom)
LieuEmprunt (CodeLieu, Nom, Commune, Contact)

#### Tables de Liaison :

APPARTENIR (ISBN, CodeGenre) [pour la relation entre Livre et Genre]
EMPRUNTER (CodeAuteur, ISBN, CodeLieu, dateEmprunt) [pour la relation entre Auteur, Livre et LieuEmprunt]

Dans cet exemple, les quatre tables principales correspondent aux entités du MCD, et deux nouvelles tables, APPARTENIR et EMPRUNTER, sont créées pour gérer les relations entre ces entités. Ces tables de liaison contiennent des références aux tables principales ainsi que des attributs supplémentaires tels que dateEmprunt pour la relation EMPRUNTER.

Il est également possible d'utiliser des outils de modélisation de bases de données tels que MySQL Workbench pour concevoir le modèle logique de données, bien que ces outils se basent souvent sur UML plutôt que Merise pour la conception.
