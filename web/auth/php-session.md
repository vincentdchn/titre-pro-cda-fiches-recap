**Fiche récapitulative : Les Sessions en PHP**

---

**Introduction**

Les sessions en PHP permettent d'associer des données à un visiteur et d'y accéder dans les scripts. Cette fiche récapitulative présente le principe de fonctionnement des sessions en PHP, notamment comment les activer, les utiliser pour stocker des données et les supprimer.

---

**Principe de Fonctionnement**

**Activer les Sessions**

Pour utiliser les sessions en PHP, il est essentiel de les activer en utilisant la fonction `session_start()`.

```php
<?php
session_start();
```

Afin d'éviter les conflits en cas de session déjà ouverte, il est recommandé de vérifier si `session_id()` est vide en utilisant `empty(session_id())` ou une méthode équivalente. Une session non démarrée entraîne `session_id` égal à une chaîne vide.

**Utiliser les Sessions**

Une fois que la fonction `session_start()` a été exécutée, vous avez accès à la superglobale `$_SESSION`, qui est un tableau permettant de stocker et d'accéder à des informations.

```php
<?php
session_start();

// Ajout d'une donnée dans le tableau de session
$_SESSION["name"] = "Philippe";
```

Plus tard, sur une autre page ou dans le même script, vous pouvez récupérer cette information :

```php
<?php
session_start();

// Affiche : Philippe
echo $_SESSION["name"];
```

**Supprimer la Session**

Vous pouvez supprimer les données stockées dans `$_SESSION` en utilisant la fonction `session_unset()`.

```php
<?php

// À ce stade, $_SESSION n'est pas définie.

// Activation des sessions, la variable $_SESSION est créée,
// avec toutes les données précédemment stockées dans d'autres scripts
session_start();

// À ce stade, $_SESSION est définie.

// Suppression des données stockées. Après un rafraîchissement de la page, $_SESSION sera vide.
session_unset();
```

**Chrome DevTools**

Dans l'onglet "Applications" du panneau de développement de Chrome (Inspecteur d'éléments), vous pouvez visualiser les cookies stockés pour chaque domaine, y compris les informations de session.

---

**Conclusion**

Les sessions en PHP sont un outil puissant pour gérer des données utilisateur entre différentes pages et sessions sur un site web. Comprendre comment activer, utiliser et supprimer des sessions est essentiel pour le développement web en PHP.
