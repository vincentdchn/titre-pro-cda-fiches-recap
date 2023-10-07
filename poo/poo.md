**Fiche Récapitulative sur les Objets en PHP**

1. **Historique et Concepts**:

    - Dans les années 1960, la programmation structurée a émergé avec des langages utilisant des structures de contrôle telles que while, repeat, for, if..then..else, et des fonctions.
    - PHP, à l'origine, était un langage de programmation procédurale centré sur l'enchaînement linéaire de code et des appels de fonctions.
    - La programmation orientée objet (POO) est née dans les années 1980-1990 pour dépasser les limitations de la programmation procédurale.
    - La POO se concentre sur la gestion des données et introduit des concepts comme l'encapsulation, l'héritage, et le polymorphisme.

2. **Programmation Orientée Objet vs. Programmation Procédurale**:

    - Programmation Structurée/Procédurale : centrée sur le code et l'enchaînement linéaire.
    - Programmation Orientée Objet : centrée sur les données, les propriétés, les méthodes, et l'organisation en entités.

3. **Avantages de la POO**:

    - Clarté fonctionnelle du code.
    - Cohérence des données et de leurs traitements associés.
    - Modularité du code.
    - Réutilisabilité du code.

4. **Concepts Clés**:

    - **Objet** : Représentation informatique d'une entité (matérielle ou immatérielle) avec des propriétés (données) et des actions (méthodes).
    - **Attribut** : Caractéristique propre à un objet, également appelée propriété.
    - **Méthode** : Action applicable à un objet qui peut modifier ses attributs.
    - **Classe** : Modèle qui définit la structure d'un objet, avec ses propriétés et méthodes.
    - **Visibilité** : Public (accès direct), Private (accès restreint aux méthodes internes de l'objet).
    - **Encapsulation** : Regrouper des données avec des méthodes pour les lire ou les manipuler, en limitant l'accès direct.

5. **Exemple de Définition d'une Classe en PHP**:

```php
class MyClass
{
    // Propriété/Attribut/Donnée
    private $property;

    // Méthode/Action/Code
    public function myMethod()
    {
        // ...
    }
}
```

6. **Instanciation d'Objets**:

    - Créer une instance (objet) à partir d'une classe avec `new`.

7. **Attributs**:

    - Déclarer et utiliser des attributs dans une classe.
    - Utiliser l'opérateur `->` pour accéder aux attributs d'un objet.

8. **Méthodes**:

    - Déclarer et appeler des méthodes dans une classe.
    - Utiliser `$this` pour référencer l'objet lui-même à l'intérieur de la classe.

9. **Visibilité**:

    - Public et Private pour contrôler l'accès aux propriétés et méthodes.
    - Préférer Private pour préserver l'encapsulation.

10. **Getters et Setters (Accesseurs et Mutateurs)**:

-   Méthodes pour accéder (getter) et modifier (setter) les propriétés privées.
-   Permettent un accès contrôlé aux données de l'objet.

11. **Méthodes Magiques PHP**:

-   `__get` et `__set` pour personnaliser le comportement lors de l'accès aux attributs.
-   Constructeur (`__construct`) et destructeur (`__destruct`) pour des actions automatiques à l'instanciation et à la destruction de l'objet.

12. **Méthodes et Propriétés Statiques**:

-   Partagées par toutes les instances de la classe.
-   Accessibles directement à partir du nom de la classe avec l'opérateur `::`.
-   Utilisation de `self` pour se référer à la classe en cours.
-   Exemple d'une propriété statique : `public static $majority;`.
-   Exemple d'une méthode statique : `public static function getMajority()`.

13. **Exemple de Propriété et Méthode Statique**:

```php
class Person
{
    private $age;

    // Propriété statique
    private static $majority;

    // Méthode statique
    public static function getMajority()
    {
        return self::$majority;
    }
}
```

14. **Constantes de Classe**:

-   Utilisées pour définir des valeurs constantes.
-   Conventions : en majuscules.
-   Accessibles à partir du nom de la classe.
-   Exemple : `const DEFAULT_NAME = "John Doe";`

15. **Opérateur de Résolution de Portée** (`::`) :

-   Utilisé pour accéder aux propriétés et méthodes statiques.
-   Exemple : `Person::getMajority();`

16. **Utilisation des Objets en PHP**:

-   Instanciation d'objets à partir de classes.
-   Accès aux attributs et méthodes à l'aide de l'opérateur `->`.
-   Encapsulation pour protéger les données et assurer leur intégrité.
-   Utilisation de méthodes statiques et de constantes de classe pour des fonctionnalités partagées.

17. **Conseils**:

-   Pratiquez la POO pour mieux comprendre et organiser votre code.
-   Utilisez l'encapsulation pour protéger vos données.
-   Évitez l'accès direct aux propriétés privées en utilisant des méthodes d'accès.
-   Utilisez les méthodes statiques pour des fonctionnalités partagées par toutes les instances de la classe.
