# Fiche récapitulative sur OAuth (Open Authorization) :

**Qu'est-ce qu'OAuth ?**

-   OAuth est un protocole d'autorisation ou un cadre (framework) qui permet aux applications d'obtenir la capacité d'accéder à des ressources désignées de manière sécurisée sans avoir à partager les mots de passe. Il permet à un utilisateur d'accorder à une application tierce l'accès à ses données sans divulguer ses identifiants.

**Différence entre SAML et OAuth :**

-   SAML (Security Assertion Markup Language) est une norme d'authentification fédérée souvent utilisée pour l'authentification unique (Single Sign-On - SSO) dans les entreprises.
-   OAuth et SAML diffèrent dans plusieurs domaines, notamment les formats de données (XML pour SAML et JSON pour OAuth), l'expérience utilisateur (OAuth est plus adapté aux applications mobiles et modernes), et l'utilisation d'API (OAuth utilise largement les appels d'API, ce qui est idéal pour les applications mobiles, les applications web modernes, les consoles de jeux, et les appareils IoT).

**Comment fonctionne OAuth ?**

-   OAuth repose sur un modèle à trois acteurs : l'utilisateur, le consommateur (consumer), et le fournisseur de services (service provider).
-   L'utilisateur autorise le consommateur à accéder à ses données sur le fournisseur de services sans divulguer son mot de passe.
-   Le consommateur obtient une autorisation temporaire (jeton d'accès) du fournisseur de services pour accéder aux données de l'utilisateur.
-   Le consommateur peut accéder aux données de l'utilisateur tant que le jeton d'accès est valide.
-   L'utilisateur peut révoquer l'autorisation à tout moment.

**OAuth 1.0 vs. OAuth 2.0 :**

-   OAuth 2.0 est une refonte complète d'OAuth 1.0 et les deux versions ne sont pas compatibles.
-   OAuth 2.0 est plus rapide, plus simple à mettre en œuvre, et prend en charge plusieurs flux pour différents types d'applications et de besoins.
-   OAuth 1.0 utilisait des exigences cryptographiques complexes, ne prenait en charge que trois flux, et ne pouvait pas évoluer aussi bien qu'OAuth 2.0.

En résumé, OAuth est un protocole d'autorisation qui permet aux utilisateurs de donner l'accès à leurs données à des applications tierces sans partager leurs identifiants. Il repose sur un modèle de jeton d'accès temporaire et est plus adapté aux applications modernes que d'autres protocoles d'authentification comme SAML. OAuth 2.0 est la version recommandée et largement utilisée aujourd'hui.
