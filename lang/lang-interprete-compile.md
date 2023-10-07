**Fiche récapitulative : Interpréter ou compiler ? La guerre des langages**

---

**Introduction**

Lorsqu'il s'agit de programmer, de nombreux langages sont disponibles, mais ils peuvent être classés en deux catégories principales : les langages compilés et les langages interprétés. Cette fiche récapitulative explore les spécificités, les avantages et les inconvénients de ces deux catégories de langages, ainsi que l'alternative des langages intermédiaires.

---

**Langage interprété**

-   Principe : Un interprète traduit chaque ligne de code en une ligne compréhensible, instruction par instruction.
-   Les interprètes sont spécifiques à chaque langage.
-   Avantages :
    -   Facilité de développement.
    -   Possibilité d'exécuter des programmes incomplets.
    -   Portabilité sur plusieurs appareils sans compilation supplémentaire.

---

**Langage compilé**

-   Principe : Un compilateur crée un fichier exécutable compréhensible par la machine. La traduction se fait en amont.
-   Processus de compilation :
    -   Analyse lexicale.
    -   Analyse syntaxique.
    -   Analyse sémantique (typage des variables).
    -   Passage en code intermédiaire.
    -   Optimisation du code intermédiaire.
    -   Génération du code final (code objet).
-   Avantages :
    -   Exécution rapide et moins coûteuse.
    -   Non lisibilité du fichier exécutable, améliorant la sécurité.
-   Inconvénients :
    -   Nécessite de recompiler après chaque modification.

---

**Comparaison**

Les différences fondamentales entre les langages interprétés et compilés résident dans les techniques de traduction et d'utilisation. Un interprète travaille en lisant et en analysant chaque instruction, tandis qu'un compilateur crée un fichier exécutable compréhensible par la machine. Les programmes interprétés sont portables, tandis que les programmes compilés offrent une exécution rapide et une sécurité améliorée.

---

**Évolution et la loi de Moore**

L'amélioration de la puissance des ordinateurs, selon la loi de Moore, a rendu les langages interprétés plus performants. Cependant, cette amélioration risque de se heurter à des limites physiques liées à la réduction de la taille des transistors.

---

**Alternative : Langages intermédiaires**

Les langages intermédiaires combinent les avantages des langages interprétés et compilés. Ils passent par une phase de compilation pour créer un fichier intermédiaire, puis par une phase d'interprétation pour exécuter le code. Cette approche permet une exécution rapide et la traduction vers différents systèmes d'exploitation.

Exemple : Java, qui compile en fichiers .class et est interprété par la machine virtuelle Java (JVM).

---

**Conclusion**

Il est difficile de trouver une solution universelle répondant à tous les besoins de programmation. Le choix entre langages interprétés, compilés ou intermédiaires dépend des objectifs du projet. Les différences tendent à se réduire avec l'évolution des ordinateurs, donc la décision doit être prise en fonction des besoins spécifiques du programme.

---

**Exemples de langages :**

**Interprétés** : Python, Ruby, Basic, Matlab, PHP, Prolog, Perl, ...

**Compilés** : C, C++, Fortran, Pascal, ...

**Intermédiaires** : Java, SQL, Eiffel, Sather...
