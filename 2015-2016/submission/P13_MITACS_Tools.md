Integration d'outils dans la plateforme CosyVerif
================================================

Résumé : Intégration et développement d'outils permettant de manipuler des automates et réseaux de Petri dans la plateforme CosyVerif.

[CosyVerif](http://cosyverif.org) est une plateforme logicielle de vérification
formelle. Développée conjointement par les laboratoires d'informatique des
universités Paris 6, Paris 13, ENS Cachan et Genève, permet la détection précoce
de problèmes difficiles (ou impossibles) à détecter par les méthodes usuelles de
test. Ces problèmes sont décrits sous formes de modèles, décrits dans des
formalismes basés sur des graphes, tels que les
[automates](https://fr.wikipedia.org/wiki/Automate) ou
[réseaux de Petri](https://fr.wikipedia.org/wiki/R%C3%A9seau_de_Petri).

L’objectif du projet est d'intégrer de nouveaux outils dans la plateforme CosyVerif.
Nous disposons d'une dizaine d'outils qui ont déjà été développés et que nous voulons rendre utilisables au travers de CosyVerif. Cependant, ils ont été intégrés au fur et à mesure des demandes.
Il en résulte un problème de cohérence : de nombreux outils rendent un services
similaire, tandis que des outils très utiles et demandés par les utilisateurs
ne sont toujours pas intégrés.

La plateforme actuelle intègre, entre autres, les outils suivants :

* [GreatSPN](http://www.di.unito.it/~greatspn/index.html), développé à
  l'université de Turin, réalise des analyses structurelles et comportementales
  des réseaux de Petri, comme la recherche d'invariants
  ou la vérification de propriétés par model checking;
* Prod, développé par l'université d'Helsinki, permet de vérifier des
  propriétés sur des réseaux de Petri, et en détaillant suffisamment ses
  résultats pour être utilisé en enseignement.

Depuis début 2015, nous développons une nouvelle version de
[CosyVerif](http://cosyverif.org). Celle-ci définit un nouveau format pour
l'intégration des outils, ce qui nous fournit l'occasion de retravailler
complètement cet aspect. Le sujet de ce projet est ainsi :

* de déterminer, avec les développeurs et utilisateurs de la plateforme,
  un ensemble cohérent d'outils à (ré)intégrer;
* d'intégrer les outils choisis ci-dessus;
* de développer des petits outils utiles aux utilisateurs mais non disponibles.

L'intégration d'un outil se fait en plusieurs étapes :

* choix du formalisme adapté (réseau de Petri, automate, ...) et extension
  de celui-ci si besoin;
* création de paquets à partir des sources de l'outil à intégrer;
* écriture d'un script permettant la conversion des entrées et sorties de
  l'outil de/vers le format utilisé par [CosyVerif](http://cosyverif.org);
* import de modèles et d'exemples d'utilisation dans la plateforme;
* écriture de tests.

Pour chaque outil intégré, une video tutorielle de démonstration de l'outil sera
enregistrée. et publiée sur Internet.

Le logiciel [CosyVerif](http://cosyverif.org) est écrit en
[Lua](ttp://www.lua.org/) sous license libre
[MIT](https://fr.wikipedia.org/wiki/Licence_MIT).

Le projet sera géré en méthode [Scrum](https://www.scrum.org/). Le projet sera
ainsi découpé en plusieurs *sprints* d'une durée fixée, correspondant chacun
à l'intégration ou au développement d'un outil, à l'issue desquels
vous enregistrerez une vidéo tutorielle présentant l'utilisation de l'outil.

Vous serez dans un environnement de développement utilisant
[GitHub](https://github.com/) pour les dépôts de sources et le suivi des
tickets, et [Shippable](https://app.shippable.com/) pour l'intégration continue.
