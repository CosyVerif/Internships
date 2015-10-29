Formalismes dans la plateforme CosyVerif
========================================

Résumé : Intégration de formalismes basés sur les automates et réseaux de Petri
dans la plateforme CosyVerif.

[CosyVerif](http://cosyverif.org) est une plateforme logicielle de vérification
formelle. Développée conjointement par les laboratoires d'informatique des
universités Paris 6, Paris 13, ENS Cachan et Genève, permet la détection précoce
de problèmes difficiles (ou impossibles) à détecter par les méthodes usuelles de
test. Ces problèmes sont décrits sous formes de modèles, décrits dans des
formalismes basés sur des graphes, tels que les
[automates](https://fr.wikipedia.org/wiki/Automate) ou
[réseaux de Petri](https://fr.wikipedia.org/wiki/R%C3%A9seau_de_Petri).

L'une des spécificités de la plateforme [CosyVerif](http://cosyverif.org) est
de permettre à l'utilisateur de créer ses propres formalismes. Afin d'aider
à leur création, la plateforme propose un ensemble de ``briques'' de
formalismes, composables entre elles.

Depuis début 2015, nous développons une nouvelle version de
[CosyVerif](http://cosyverif.org), dans laquelle le format de description
des modèles et formalismes a changé. Le but de ce projet et d'ajouter un
certain nombre de formalismes utiles à la plateforme :

* certains types d'automates et de réseaux de Petri;
* certains types de logiques temporelles
  ([CTL](https://en.wikipedia.org/wiki/Computation_tree_logic),
   [LTL](https://en.wikipedia.org/wiki/Linear_temporal_logic), ...);
* des formalismes modulaires et hiérarchiques récemment publiés, par exemple
  [Modular PNML](https://lipn.univ-paris13.fr/applications/publications/fichiers/EK-LP-ATPN09.pdf).

Les formalismes sont représentés sous forme de structures de données écrites en
langage [Lua](http://www.lua.org/). Celui-ci est suffisamment simple pour être
appris au cours du projet de recherche.
