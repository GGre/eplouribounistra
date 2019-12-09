# AppliWeb collaborative pour gérer le dédoublonnement des revues dans les bibliothèques.

Gagnez de l'espace en éliminant vos doublons, offrez une meilleure lisibilité de vos ressources en reconstituant pour chacune d'elles une collection unique la plus intègre possible résultant de l'agrégation des éléments épars disponibles dans vos bibliothèques.

# Méthode :

Pour une ressource donnée (Unité catalographique sans les filiations), l'application eplouribousse permet aux bibliothèques, chacune à son tour, d'indiquer ses éléments reliés contribuant à la résultante, puis lors d'un deuxième cycle d'instructions et selon la même logique, ses éléments non-reliés complémentaires.

L'ordre de traitement est significatif : La première bibliothèque est normalement celle détenant déjà la collection la plus importante (Celle qui revendique la conservation dans l'hypothèse où la collection est finalement regroupée). C'est la même logique d'importance qui doit prévaloir normalement pour la place revendiquée par les bibliothèques suivantes. Il peut arriver qu'une bibliothèque veuille soustraire sa collection à la reconstitution de la résultante (Le cas typique est celui d'une collection du dépôt légal) Le module de positionnement de l'application eplouribousse rend cette dérogation possible.

Les fiches obtenues décrivent les résultantes ; les éléments écartés s'en déduisent. Les parties contribuant à la collection résultante peuvent être regroupées ou pas, au choix. Les traitements physiques et mises à jour catalographiques sont à prévoir.

(Voir le poster réalisé pour les journées de l'ABES 2014 : https://seafile.unistra.fr/f/a7e47cd0a17c46ea8ee9/)

# Fonctionnalités :

01. édition des candidats pour chaque bibliothèque participante,
02. formulaire de positionnement (ou de dérogation),
03. édition des ressources dont l'instruction de la résultante peut débuter,
04. alerte quand son tour est venu de poursuivre l'instruction de la résultante,
05. formulaires d'instruction (ajout, suppression, fin),
06. édition différenciée des résultantes (rapports soignés au format pdf),
07. contrôle de conformité à la fin de chaque cycle d'instruction,
08. prise en charge complète de la chaîne de traitement,
09. tableau de suivi d'activité,
10. gestion des utilisateurs,
11. contrôles d'authentification,
12. paramétrage des motifs de dérogation,
13. administration des cas de fiches défectueuses,
14. prise en charge multilingue (français, anglais, allemand ; possibilité d'étendre à d'autres langues)

# Plus d'info :

Voir le manuel de l'appli en https://seafile.unistra.fr/f/a998b238a22b4c13baf5/

# Comment obtenir eplouribousse ?

Pour avoir un aperçu de l'application, commencez par visiter une instance réelle : https://eplouribousse.di.unistra.fr/

----------------

ça vous a plu ? Allez plus loin ; essayez eplouribousse sur un poste local équipé du serveur de développement de Django ; cela vous permettra de tester toutes les fonctionnalités (à l'exception des alertes mail qui ne sont qu'une commodité)

Pour cela, clonez le dépôt https://github.com/GGre/eplouribounistra dans un répertoire de votre choix, puis téléchargez le specimen de base de données https://seafile.unistra.fr/f/c9a7a7dfa00a417ebb24/?dl=1

Décompressez et placez la base de données eplouribousse.db dans le répertoire qui contient le fichier manage.py
(Un petit coup d'oeil sur la structure de la base vous permettra d'élaborer la vôtre)

Dans un terminal, placez-vous dans le répertoire contenant le fichier manage.py, lancer la commande : export DJANGO_SETTINGS_MODULE=eplouribousse.settings.dev

puis lancer le serveur de développement : python manage.py runserver (ou éventuellement : python3 manage.py runserver)

Testez !

En cas de demande d'authentification, l'identifiant est le prénom et le mot de passe temporaire est testeplou (quel que soit l'identifiant)

Pour ce test, nous avons trois bibliothèques : Jean travaille pour la bibliothèque "Les Jouvencelles", Suzanne pour la bibliothèque "La Combe du Lac", Pierrette pour la bibliothèque "La Serra" ; Claire est le vérificateur ; Flora administre la base de données, Alain administre le site et vous, vous êtes Jules le super-utilisateur. Découvrez ce que chacun peut faire, quels sont ses droits, comment il peut interagir avec l'application.

----------------

Vous êtes convaincu et vous voulez mettre en oeuvre eplouribousse dans votre établissement ?
Nous conseillons d'abord de vous rapprocher de votre équipe informatique pour une installation de test.

Si vous souhaitez utiliser eplouribousse pour un projet ferme, il y a actuellement trois possibilités :
- Confier le déploiement à votre service informatique en indiquant l'adresse du présent site
- Confier le déploiement à un hébergeur en indiquant l'adresse du présent site
- Nous confier le déploiement (sous réserve d'accord)

Dans tous ces cas, veuillez nous informer de votre intérêt (contact ci-après)

# Contact :

Indiqué en https://github.com/GGre/eplouribounistra/blob/master/Version.txt

