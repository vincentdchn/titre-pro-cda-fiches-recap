# Fiche récapitulative des informations essentielles sur JSON Web Tokens (JWT) :

**Qu'est-ce que JSON Web Token (JWT) ?**

-   JWT est une norme ouverte (RFC 7519) qui définit un moyen compact et autonome de transmettre de manière sécurisée des informations entre les parties sous forme d'objet JSON.
-   Les JWT peuvent être signés à l'aide d'une clé secrète (avec l'algorithme HMAC) ou d'une paire de clés publique/privée (RSA ou ECDSA).
-   Ils peuvent également être chiffrés pour fournir la confidentialité, mais nous nous concentrons sur les tokens signés ici.

**Quand utiliser JSON Web Tokens ?**

-   JWT est couramment utilisé pour l'authentification, permettant à un utilisateur d'accéder aux routes, services et ressources autorisées après la connexion.
-   Il est également utilisé pour l'échange sécurisé d'informations entre les parties, grâce à la signature numérique.

**Structure d'un JSON Web Token :**

-   Un JWT se compose de trois parties séparées par des points (.) : Header, Payload et Signature.

**Header :**

-   Contient le type de token (JWT) et l'algorithme de signature utilisé (par exemple, HS256).

**Payload :**

-   Contient des affirmations (claims) sur une entité, telles que l'émetteur (iss), le temps d'expiration (exp), le sujet (sub), l'audience (aud), ainsi que des claims personnalisés.

**Signature :**

-   Calculée en utilisant le header et le payload encodés, une clé secrète et l'algorithme spécifié dans le header.

**Fonctionnement des JSON Web Tokens :**

-   Après la connexion réussie d'un utilisateur, un JWT est renvoyé.
-   L'utilisateur envoie le JWT dans l'en-tête Authorization pour accéder aux ressources protégées.
-   Le serveur vérifie la validité du JWT et autorise l'accès en conséquence.

**Pourquoi utiliser JSON Web Tokens ?**

-   Avantages par rapport à d'autres formats de jetons : plus compact, supporte la signature avec des paires de clés publique/privée, facilité de traitement côté client sur différentes plateformes, et plus simple à manipuler que XML.
