Paquito
=======

Paquito est un outil permettant de construire facilement des paquets (Debian,
Red Hat, Mac, ...) à partir des sources d'un logiciel et d'un fichier de
configuration.

Cet outil a été développé de 2013 à 2015 au cours de deux stages
d'été. Il permet actuellement de construire des paquets pour différents
systèmes Linux. Nous l'utilisons pour deux logiciels développés dans des
laboratoires de recherche : [CosyVerif](http://cosyverif.org), projet conjoint
des universités Paris 6, Paris 13, ENS Cachan et Université de Genève,
et [Orchids](http://www.lsv.ens-cachan.fr/Software/orchids/v2.1/), un projet
de l'ENS Cachan financé (entre autres) par la
[DGA](http://www.defense.gouv.fr/dga]).

Cependant, plusieurs améliorations restent à développer pour qu'il soit
réellement utilisable :

* construction de paquets pour Mac;
* amélioration de la gestion des dépendances;
* extraction automatique de certaines informations (version, auteurs, ...)
  depuis les gestionnaires de versions ([git](https://git-scm.com/),
  [subversion](https://subversion.apache.org/), ...);
* extraction automatique d'informations (mainteneur, organisation, ...)
  depuis les services d'hébergement de logiciels, tels que
  [GitHub](https://github.com/) ou [BitBucket](https://bitbucket.org/);
* création d'un service web connecté à [GitHub](https://github.com/)
  permettant de lancer la construction des paquets à chaque `push` ou `tag`;
* création d'une interface web autour de ce service;
* et bien sûr des tests pour toutes ces fonctionnalités, avec une bonne
  couverture de code.

Le logiciel Paquito est écrit en [PHP](http://php.net/) sous licence libre
[MIT](https://fr.wikipedia.org/wiki/Licence_MIT). Les fichiers de configuration
sont au format [YAML](http://yaml.org/). Pour générer les paquets, Paquito
utilise des conteneurs [Docker](https://www.docker.com/).

Le projet sera géré en méthode [Scrum](https://www.scrum.org/).Le projet sera
ainsi découpé en plusieurs *sprints* d'une durée fixée, à l'issue desquels
vous montrerez les fonctionalités implémentées.

Vous serez dans un environnement de développement utilisant
[GitHub](https://github.com/) pour les dépôts de sources et le suivi des
tickets, et [Shippable](https://app.shippable.com/) pour l'intégration continue.
Vous devrez proposer une architecture simple, propre et modulaire.
L'implémentation devra être maintenable, claire et respecter les standards
[PSR](http://www.php-fig.org/psr/).
