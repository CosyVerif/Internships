Client Web pour CosyVerif
=========================

Développement d'un client web pour la plateforme CosyVerif

[CosyVerif](http://cosyverif.org) est une plateforme logicielle de vérification
formelle. Développée conjointement par les laboratoires d'informatique des
universités Paris 6, Paris 13, ENS Cachan et Genève, permet la détection précoce
de problèmes difficile (ou impossible) à détecter par les méthodes usuelles de
test.

Les outils intégrés dans [CosyVerif](http://cosyverif.org) sont très gourmands
en mémoire, ainsi qu'en temps de calcul. C'est pourquoi ils sont exécutés sur
de grosses machines dédiées. La plateforme est ainsi construire sur un modèle
client/serveur. Le client doit être simple à installer et utiliser, ainsi
qu'être portable.

Depuis début 2015, nous développons une nouvelle version de cette plateforme.
Pour cela, nous utilisons les standards du Web lorsque c'est possible. Par
exemple, les communications se font par
[WebSockets](https://www.websocket.org/).

L’objectif du projet est de développer un client Web plateforme CosyVerif
 qui permet notamment d'invoquer des outils qui manipulent des réseaux de Pétri et des Automates.
Le client permet d'abord de définir et sélectionner les formalismes des modèles puis de définir des modèles dans ces formalismes.
Le client pourra ensuite charger des outils hébergés dans CosyVerif puis les invoquer afin de conduire les expérimentations
 qui permettrons notamment d'établir des preuves basées sur les informations structurelles du modèle.

Vous avez la chance d'integrer un projet novateur qui offre une visibilité mondiale
 qui permet de mettre le doigt sur des outils développés à l'International.
Les développements se font en langage Lua sur Linux ou MacOS, en utilisant la méthodologie scrum
   et l'intégration continue avec Shippable.
     avec le SCM git et gitHub,  test unitaires avec busted
A chaque fin de sprint vous enregistrez une video qui démontrera les fonctionnalités de votre client.
