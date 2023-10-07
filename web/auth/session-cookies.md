**Fiche récapitulative : Conservez des Données grâce aux Sessions et aux Cookies en PHP**

---

**Introduction**

Ce résumé porte sur la conservation des données entre différentes pages PHP en utilisant les sessions et les cookies. Les sessions et les cookies sont des méthodes essentielles pour stocker et accéder à des informations persistantes sur un site web.

---

**Conservez les Données grâce aux Sessions**

-   Les sessions permettent de stocker des variables sur toutes les pages d'un site web pour une durée de visite donnée.
-   Le fonctionnement des sessions en PHP se compose de trois étapes : création d'une session unique, création de variables pour la session, et suppression de la session.
-   La fonction `session_start()` est utilisée pour démarrer le système de sessions, tandis que `session_destroy()` permet de fermer la session du visiteur.
-   Les sessions peuvent être utilisées pour conserver des informations telles que l'authentification d'un utilisateur, la création de zones d'administration sécurisées, la gestion de paniers d'achat, etc.

**Conservez les Données grâce aux Cookies**

-   Les cookies sont de petits fichiers texte stockés sur l'ordinateur du visiteur et utilisés pour retenir des informations.
-   Chaque cookie stocke généralement une information à la fois.
-   Pour écrire un cookie en PHP, on utilise la fonction `setcookie()`, qui nécessite généralement trois paramètres : le nom du cookie, sa valeur, et la date d'expiration (timestamp).
-   Les cookies peuvent être sécurisés en utilisant les options `httpOnly` et `secure` pour prévenir les failles XSS.
-   Pour récupérer le contenu d'un cookie en PHP, on accède au tableau `$_COOKIE`, par exemple : `$_COOKIE['nom_cookie']`.

**Conclusion**

Les sessions et les cookies sont des outils puissants pour conserver des données entre différentes pages et sessions sur un site web. Ils sont largement utilisés pour l'authentification, la gestion de paniers d'achat, la personnalisation des expériences utilisateur, et bien plus encore. Comprendre comment utiliser ces mécanismes est essentiel pour développer des fonctionnalités interactives et dynamiques sur un site web en PHP.
