# Fiche récapitulative : Événements en JavaScript

---

**Événements**

JavaScript est un langage axé sur la gestion des interactions entre l'utilisateur et le navigateur. Les événements utilisateurs tels que les clics, les défilements, et la soumission de formulaires sont des actions auxquelles un développeur peut associer du code pour définir leur comportement.

---

**addEventListener**

La méthode `addEventListener` permet de créer un écouteur d'événement, c'est-à-dire une fonction qui indique au navigateur comment réagir à des événements futurs d'un certain type. Voici sa syntaxe :

```javascript
element.addEventListener(eventType, handler);
```

-   `element` est une référence vers un nœud du DOM.
-   `eventType` est une chaîne de caractères décrivant le type d'événement à surveiller.
-   `handler` est une fonction anonyme (`function() { ... }`) ou une référence à une fonction existante.

Exemple :

```javascript
const element = document.getElementById('inscription');

const subscribeUser = function () {
    // Code pour enregistrer l'inscription de l'utilisateur
};

element.addEventListener('click', subscribeUser);
```

---

**Objet-événement**

Le handler, aussi appelé callback ou gestionnaire d'événement, est une fonction qui sera automatiquement appelée par le navigateur en réaction à un événement précis. Il peut accepter un objet décrivant l'événement survenu comme paramètre, envoyé par le navigateur :

```javascript
const subscribeUser = function (evt) {
    console.log(evt);
    // Code pour enregistrer l'inscription de l'utilisateur
};
```

L'objet-événement contient de nombreuses informations utiles sur l'événement, notamment la méthode `preventDefault`, qui permet de bloquer le comportement par défaut du navigateur dans certains cas, comme la soumission de formulaires.

Exemple d'utilisation de `preventDefault` :

```javascript
document
    .getElementsByTagName('form')[0]
    .addEventListener('submit', function (evt) {
        evt.preventDefault(); // Empêche le rechargement automatique de la page
        // Le code peut s'exécuter maintenant...
    });
```

---

**Types d'événements**

Il existe de nombreux types d'événements auxquels vous pouvez réagir. Vous pouvez même créer vos propres types avec `new Event('montype')`. Pour obtenir une liste des types d'événements disponibles, consultez la documentation [MDN sur les types d'événements](MDN).

---

**Handler et traitement d'informations**

Un handler peut être exécuté plusieurs fois pour un même événement, il est donc essentiel de le concevoir de manière autonome, sans dépendre d'informations persistantes entre les appels. L'objet-événement passé en paramètre, généralement nommé `event` ou `evt`, contient des informations sur l'événement en cours.

L'objet-événement permet d'accéder à l'élément du DOM qui a déclenché l'événement via `evt.target`. Vous pouvez également utiliser les attributs `data-` pour transmettre des informations spécifiques du HTML au JavaScript, ce qui est exploitable dans le handler.

---

**Supprimer un écouteur d'événement**

Pour retirer un écouteur d'événement d'un élément HTML, vous devez spécifier l'élément, le type d'événement et le handler :

```javascript
bouton.removeEventListener('click', cliqueBouton);
```

---

Cette fiche récapitulative couvre les concepts fondamentaux des événements en JavaScript, y compris l'ajout d'écouteurs, la gestion des objets-événements, les types d'événements, la conception de handlers et la suppression d'écouteurs. Utilisez ces informations pour vous préparer à votre entretien sur les événements en JavaScript.
