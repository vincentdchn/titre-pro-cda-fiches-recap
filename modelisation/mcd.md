Le Modèle Conceptuel de Données, également connu sous le nom de Modèle Entité-Association (EA), est une représentation rigoureuse d'un système de données ou d'informations. Il se base sur des entités et les relations qui les lient. Voici les éléments clés du MCD :

## Entités :

Les entités sont représentées par des rectangles.
Elles sont nommées au singulier ou au pluriel, mais pas les deux mélangés.
Chaque entité a des attributs qui sont les données la concernant.
Un attribut unique, appelé le déterminant ou discriminant, permet d'identifier de manière unique chaque instance d'entité. La clé primaire est utilisée dans la base de données pour cela.

## Associations :

Les associations sont représentées par des rectangles arrondis et nommées par un verbe à l'infinitif.
Les verbes peuvent être à l'infinitif, à la forme passive ou accompagnés d'un adverbe.
Les clés étrangères ne sont pas incluses dans le MCD.
Les attributs techniques tels que "Created at" et "Updated at" ne sont pas inclus, sauf s'ils sont intrinsèques à une entité.

## Cardinalités :

Les cardinalités définissent les quantités minimum et maximum de relations entre deux entités A et B, de A vers B et de B vers A.
Il existe quatre valeurs possibles pour les cardinalités : (0,1), (1,1), (0,n), (1,n).
Les cardinalités maximales sont privilégiées pour nommer la relation, soit "un à plusieurs" (1,n) soit "plusieurs à plusieurs" (n,n).

## Raccourcis de langage :

Les cardinalités maximales (1,n et n,n) ont un impact significatif sur l'implémentation physique et influencent souvent le nom de la relation.
Les relations "un à plusieurs" (1,n) et "plusieurs à plusieurs" (n,n) sont couramment utilisées.

## Autres cas d'association :

Parfois, des attributs de relation, tels que le rôle d'une personne dans un film, font partie de l'association.
Les associations peuvent impliquer plusieurs occurrences d'une même entité.
Les relations n-aires impliquent plus de deux entités.

## Association réflexive :

Une association réflexive se produit lorsque des occurrences d'une même entité se font référence entre elles.
Par exemple, des catégories qui ont des catégories parentes et/ou des catégories enfants sont des exemples d'associations réflexives.
Le MCD est une étape cruciale dans la conception d'une base de données, permettant de définir de manière précise la structure des données et les relations entre les entités pour répondre aux besoins d'une application ou d'un système d'informations.
