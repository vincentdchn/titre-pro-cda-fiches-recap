**Fiche récapitulative : Protocole HTTP (HyperText Transfer Protocol)**

---

**Introduction**

Le protocole HTTP (HyperText Transfer Protocol) est essentiel dans la communication entre les clients (comme les navigateurs Web) et les serveurs sur Internet. Cette fiche récapitulative présente les concepts fondamentaux de HTTP, notamment la structure des requêtes et des réponses, les méthodes HTTP et leur signification.

---

**HTTP : Requête et Réponse**

HTTP fonctionne sur un modèle de demande/réponse. Le client envoie une requête au serveur, qui répond avec une réponse. Chacune de ces requêtes et réponses est composée d'en-têtes (headers) et d'un contenu (body).

---

**Requête HTTP**

Les en-têtes de requête contiennent des informations essentielles pour que le serveur puisse traiter la requête. Les éléments courants dans les en-têtes de requête incluent :

-   Méthode HTTP (GET, POST, etc.)
-   URL
-   Version du protocole HTTP
-   Domaine de destination (host)
-   Cookies
-   Paramètres
-   Types de réponses acceptés (HTML, JSON, etc.)

Exemple de requête HTTP :

```
GET / HTTP/1.1
Host: oclock.io
Connection: keep-alive
[...]
```

---

**Corps de Requête**

Pour les requêtes de type POST (typiquement pour les formulaires), le corps de la requête contient les données à transmettre au serveur. Le corps suit les en-têtes de requête après un saut de ligne.

Exemple de corps de requête :

```
email=john%40oclock.io&name=John
```

---

**Réponse HTTP**

Une réponse HTTP contient également des en-têtes et un corps. Les en-têtes de réponse comprennent :

-   Version du protocole HTTP
-   Code de statut HTTP
-   Cookies à définir (si nécessaire)
-   Types de contenu envoyés
-   Informations utiles pour le client

Exemple de réponse HTTP :

```
HTTP/1.1 200 OK
Date: Sun, 16 Apr 2017 10:35:54 GMT
Server: Apache/2.4.10 (Debian)
Content-Type: text/html; charset=utf-8
[...]
```

---

**Méthodes HTTP et Leur Signification**

Lors de la requête, le client spécifie la méthode HTTP à utiliser. Cette méthode précise comment les informations sont envoyées au serveur et l'objectif de la requête. Voici les méthodes HTTP courantes et leur signification :

-   GET : Accéder à une ressource (lecture).
-   POST : Insérer des données côté serveur.
-   PUT ou PATCH : Mettre à jour ou insérer des données côté serveur.
-   DELETE : Supprimer des données côté serveur.

La plupart des navigateurs modernes ne prennent en charge que POST et GET dans les formulaires HTML, tandis que les autres méthodes sont utilisées avec XMLHttpRequest.

---

**Conclusion**

Cette fiche récapitulative met en lumière les principaux concepts du protocole HTTP, notamment sa structure de requête et de réponse, les en-têtes et les méthodes HTTP. Comprendre HTTP est essentiel pour toute personne travaillant sur le développement Web ou la communication client-serveur sur Internet.
