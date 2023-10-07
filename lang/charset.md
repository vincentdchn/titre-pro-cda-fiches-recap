**Fiche récapitulative : Paramètre HTTP Charset**

---

**Introduction**

Lorsqu'un serveur envoie un document à un agent utilisateur, il transmet également des informations sur le format des données via l'entête HTTP Content-Type. Une de ces informations essentielles est le paramètre charset, qui spécifie le codage du document. Cette fiche récapitulative traite de l'importance du paramètre charset dans l'entête HTTP, de la manière de le configurer sur le serveur, et de son utilisation dans divers langages de script côté serveur.

---

**Le Paramètre Charset**

Le paramètre charset est utilisé pour spécifier le codage d'un document dans l'entête HTTP. Pour les documents texte tels que text/html, text/plain, etc., il est essentiel de spécifier le charset pour une interprétation correcte par l'agent utilisateur.

---

**Configuration du Serveur**

La configuration du serveur pour envoyer les informations de charset correctes dépend du logiciel serveur utilisé. Voici quelques exemples :

-   **Apache**: Utilisez les directives AddCharset, AddType ou AddDefaultCharset dans le fichier de configuration ou le fichier .htaccess pour spécifier le charset.

-   **Jigsaw**: Utilisez un indexer dans JigAdmin pour associer les extensions de fichiers aux charsets ou configurez directement le charset sur une ressource.

-   **IIS (Internet Information Services) 5 et 6**: Dans le gestionnaire des services Internet, configurez les entêtes HTTP pour spécifier le charset associé aux extensions de fichiers.

---

**Langages de Scripts et Entête HTTP**

Il est également possible de spécifier le charset dans l'entête HTTP en utilisant des langages de script côté serveur. Voici des exemples pour différents langages :

-   **Perl**: Utilisez la fonction print pour renvoyer l'entête HTTP avec le charset spécifié.

-   **Python**: Utilisez une syntaxe similaire à Perl pour renvoyer l'entête HTTP.

-   **PHP**: Utilisez la fonction header() pour spécifier le Content-type et le charset.

-   **Servlets Java**: Utilisez la méthode setContentType de ServletResponse avant d'obtenir un objet de sortie.

-   **JSP (JavaServer Pages)**: Utilisez la directive de page pour spécifier le contentType avec le charset.

-   **ASP (Active Server Pages) et ASP.Net**: Utilisez les objets Response pour définir le ContentType et le Charset.

---

**Conclusion**

Le paramètre charset dans l'entête HTTP est essentiel pour garantir que les documents texte sont correctement interprétés par les agents utilisateurs. Sa configuration dépend du serveur utilisé, et il peut également être spécifié en utilisant des langages de script côté serveur. Une utilisation correcte du charset améliore la compatibilité et la lisibilité des pages Web.
