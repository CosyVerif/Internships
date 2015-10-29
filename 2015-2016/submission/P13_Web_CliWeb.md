Client Web pour CosyVerif
=========================

Développement d'un client web pour la plateforme CosyVerif

[CosyVerif](http://cosyverif.org) est une plateforme logicielle de vérification
formelle. Développée conjointement par les laboratoires d'informatique des
universités Paris 6, Paris 13, ENS Cachan et Genève, permet la détection précoce
de problèmes difficile (ou impossible) à détecter par les méthodes usuelles de
test. Ces problèmes sont décrits sous formes de modèles,
[automates](https://fr.wikipedia.org/wiki/Automate) ou
[réseaux de Petri](https://fr.wikipedia.org/wiki/R%C3%A9seau_de_Petri).

Les outils intégrés dans [CosyVerif](http://cosyverif.org) sont très gourmands
en mémoire, ainsi qu'en temps de calcul. C'est pourquoi ils sont exécutés sur
de grosses machines dédiées. La plateforme est ainsi construire sur un modèle
client/serveur. Le client doit être simple à installer et utiliser, ainsi
qu'être portable.

Depuis début 2015, nous développons une nouvelle version de cette plateforme.
Pour cela, nous utilisons les standards du Web lorsque c'est possible. Par
exemple, les communications se font par
[WebSockets](https://www.websocket.org/).

L’objectif du projet est de développer un client Web pour la plateforme
[CosyVerif](http://cosyverif.org). Nous disposons déjà d'un prototype; les
choix technologiques sont ainsi déjà faits et seront imposés. Le serveur
étant développé en langage [Lua](http://www.lua.org/), le code côté client web
devra être écrit dans ce même langage, à la place de
[JavaScript](https://fr.wikipedia.org/wiki/JavaScript). Ceci n'est pas un
problème car une bibliothèque d'interaction entre les deux langages existe :
[lua.vm.js](https://kripken.github.io/lua.vm.js/lua.vm.js.html).

Le client Web de CosyVerif est décomposé en deux parties :

* une interface de gestion des utilisateurs, modèles, et outils;
* une interface d'édition des modèles, permettant une édition collaborative
  de graphes annotés au moyen de la bibliothèque [d3.js](http://d3js.org/).

Elles sont relativement indépendantes et nécessitent des compétences
différentes.

Le logiciel [CosyVerif](http://cosyverif.org) est écrit en
[Lua](ttp://www.lua.org/) sous license libre
[MIT](https://fr.wikipedia.org/wiki/Licence_MIT).

Le projet sera géré en méthode [Scrum](https://www.scrum.org/). Le projet sera
ainsi découpé en plusieurs *sprints* d'une durée fixée, à l'issue de laquelle
vous enregistrerez une video qui démontrera les fonctionnalités de votre client.

Vous serez dans un environnement de développement utilisant
[GitHub](https://github.com/) pour les dépôts de sources et le suivi des
tickets, et [Shippable](https://app.shippable.com/) pour l'intégration continue.
Vous devrez proposer une architecture simple, propre et modulaire.
L'implémentation devra être maintenable, claire et respecter les standards.
