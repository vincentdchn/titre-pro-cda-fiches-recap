# Fiche recapitulative concepts de Dependency Injection (DI), Dependency Inversion (DI), et Inversion of Control (IoC) :

**Inversion de Contrôle (IoC)**

-   IoC est un principe de programmation qui inverse le flux de contrôle dans une application.
-   Dans la programmation procédurale traditionnelle, le code principal instancie des objets, appelle des méthodes, et gère le flux d'exécution.
-   Avec IoC, un framework prend en charge l'instanciation, les appels de méthodes et le déclenchement d'actions utilisateur, déplaçant la responsabilité du code principal.
-   Cette inversion de contrôle permet aux frameworks de servir de squelettes extensibles.

**Dependency Injection (DI)**

-   DI est une technique de conception logicielle où la création et la liaison des dépendances se font en dehors de la classe dépendante.
-   Les dépendances sont fournies déjà instanciées et prêtes à être utilisées, ce qui évite à la classe dépendante d'avoir à les instancier elle-même.
-   Les types d'injection DI incluent l'injection par constructeur, l'injection par interface, et l'injection par setter.
-   DI sépare la construction et la configuration des services de leur utilisation, améliorant la réutilisabilité et la facilité de test.

**Principe d'Inversion de Dépendance (DIP)**

-   DIP est un principe formulé par Robert Martin, a.k.a. Uncle Bob, qui énonce que les modules de haut niveau ne devraient pas dépendre des modules de bas niveau, mais plutôt des abstractions.
-   Les abstractions ne doivent pas dépendre des détails, les détails doivent dépendre des abstractions.
-   Cela signifie que les classes de haut niveau dépendent des abstractions, et les classes de bas niveau dépendent également des abstractions.
-   L'inversion de dépendance conduit à une meilleure modularité et à la facilité de remplacement des implémentations.

En résumé, IoC est un principe fondamental utilisé par les frameworks pour inverser le contrôle du flux dans une application, DI est le modèle utilisé pour fournir des dépendances à une classe, et le Principe d'Inversion de Dépendance (DIP) encourage la dépendance des abstractions plutôt que des détails concrets. Tous ces concepts contribuent à la réduction du couplage et à l'amélioration de la modularité dans le développement logiciel.
