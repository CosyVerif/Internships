Integration d'outils dans la plateforme CosyVerif
================================================

Résumé : Intégration de plusieurs outils permettant de manipuler des automates et réseaux de Petri dans la plateforme CosyVerif.

[CosyVerif](http://cosyverif.org) est une plateforme logicielle de vérification
formelle. Développée conjointement par les laboratoires d'informatique des
universités Paris 6, Paris 13, ENS Cachan et Genève, permet la détection précoce
de problèmes difficiles (ou impossibles) à détecter par les méthodes usuelles de
test. Ces problèmes sont décrits sous formes de modèles, décrits dans des
formalismes basés sur des graphes, tels que les
[automates](https://fr.wikipedia.org/wiki/Automate) ou
[réseaux de Petri](https://fr.wikipedia.org/wiki/R%C3%A9seau_de_Petri).

L’objectif du projet est d'intégrer de nouveaux outils dans la plateforme CosyVerif.
Nous disposons d'une dizaine d'outils qui ont déjà été développés et que nous voulons rendre utilisables au travers de CosyVerif.

Par exemple l'outil greatSPN qui a été développé à l'université de Turin va nous permettre de faire des analyses structurelles des propriétés des réseaux de Petri P/T
  comme la recherche d'invariants.

Un autre exemple est l'outil Prod qui a été développé par l'université d'Helsinki et qui va nous permettre de faire
 des vérifications sur des réseausx de Petri symétriques, (Recherche de chemins, Dead locks, Graphe d'atteignabilité...)

La plateforme CosyVerif est écrite en langage [Lua](http://www.lua.org/). Celui-ci est suffisamment simple pour être
appris au cours du projet de recherche.
L'intégration des outils se fera en développant des services d'intégration.

Pour chaque outil intégré, une video tutorielle de démonstration de l'outil sera enregistrée. et publiée sur Internet.

