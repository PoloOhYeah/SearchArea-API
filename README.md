Cette documentation contient tout ce qu'il faut savoir pour utiliser correctement l’API et savoir la mettre en place correctement sur vos serveurs ou via nos serveurs.

Dans ce document, plusieurs points seront évoqués pour expliquer au mieux le fonctionnement de l’API SearchArea.

Des annexes seront également disponibles dans la documentation pour mieux illustrer les explications.

Le fonctionnement de base du script et simple comme bonjour, il est basé sur la bibliothèque « fuse.js » qui est open source est développé par Kiro Risk sur GitHub. Fuse.js est une bibliothèque qui permet une recherche beaucoup plus précise mais comme même assez floue par rapport a des moteur de recherche traditionnel.

Il fonctionnement de manière séparé via le fichier script.js qui inclus tout l’index des recherches que le moteur connais. Le script prend cet forme là :


Dans la première ligne il récupère la fonction openPage puis la transmet a la fonction getElementById qui la fait corespondre au mieux a l’index entier pour trouver le meilleure résultat, Nous pouvons voir que sur le premier exemple avec le terme de recherche « Gironde » pointe sur gironde.html mais un deuxieme terme de recherche a été ajouté qui est « Incendie Gironde », il est ajouté car le script fuse.js dispose d’une limite parce que si ont lui donne trop de mot il risque de pointer un autre fichier autre que celui attendu par l’utilisateur :

Exemple :

Si je tape dans la barre de recherche « Incendie dans la gironde », il peut toujours me pointer vers le bon résultat, mais si je tape « Incendie dans un camping en gironde », là il pourra moins bien comprendre ceux que l’utilisateur demande et pourra peut être rediriger vers Camping ou Gironde.


Le script peut également mieux comprendre les fautes d'orthographe , il pourra essayer de faire le maximum pour faire correspondre les mots et lettres vers les résultats.

Exemple :

Hunter X Hunter ⇒ hunterxhunter.html

Hunter Hunter ⇒ hunterxhunter.html

Hunteer X Huunter ⇒ hunterxhunter.html

Hunr X Hunteer ⇒ hunterxhunter.html

Pour les trois version du terme de recherche, cela est une réussite et pointe toujours sur le bon fichier.



Ensuite le script vérifie en un instant la correspondance avec le terme de recherche puis via la dernière ligne ouvre le bon fichier dans un nouvel onglet et vous affiche les résultats de recherche.


Les principales différence avec l’API et le script de base est une meilleure sécurité lors des requêtes et permet une meilleure interaction avec le site pour de meilleure recherche.

De plus l’API pourra être inclus sur votre propre site web ou tout autre site pour pouvoir faire des recherche sur votre site ou même en rapport avec votre site pour que vos utilisateurs puisse se renseigner gratuitement depuis votre site via nos services.

Vous pouvez nous envoyez un e-mail ou nous contacté via notre formulaire pour une demande pour faire votre propre moteur de recherche pour votre site ou porte folio.


L’API sera disponible sous différente forme comme une simple barre de recherche ou vous pouvez faire votre propre barre de recherche est inclure le script, noté que le logo de SearchArea doit être présent soit au dessus de la barre de recherche, en petit ou mentionner quelque part dans le pied de page.
Si aucune indication ne redirige vers SearchArea, votre accès a l’API sera bloqué jusqu’à nouvel ordre et cela manuellement par nos équipes.



Cet API de SearchArea si ont peut dire ça, pourra vous permettre que récupérer directement des pages du moteur sans passer par l’interface ou bien de faire des demandes de moteur personnalisé pour vos pages web ceux qui pourra permettre a l’utilisateur de faire une recherche approfondie du sujet ou du site lui même sur lequel vous êtes.


Cela reste évidement un exemple, l’utilisateur peut mettre la barre de recherche ou il veut sur sa page web.

Les prochaines pages de la documentation seront là pour détaillé le fonctionnement de l’API.

L’API utilise des scripts différents pour chaque type d’utilisation, le script utilise le même pattern que celui de base :


Mais il est adapté au site du commanditaire ou du particuliers qui demande l’API, si l’utilisateur en fait la demande, il peut permettre la recherche sur l’ensemble du moteur de recherche, parce que par défaut l’API ne fonctionnera que avec des résultats du commanditaire ou du particuliers.

L’API pourra alors contenir plus ou moins tous pleins de résultats de recherches concernant le sujet du site ainsi que des documents et images. Par exemple si c’est la SNCF, il peut y avoir différents site mentionnant la SNCF comme des articles ou des sites affiliés comme Transilien ou IDFM mais les résultats seront uniquement centré sur SNCF et non d’autres termes de recherche.

Pour l’utilisation de l’API ou de ce service là du site, Area SafeSearch ne sera pas activer par défaut, ça sera a l’utilisateur d’en faire la demande.

De plus, plusieurs autre services ou fonctionnalités pourront être inclus sur l’API comme la recherche directement d’images, de documents ou SafeSearch directement.
La personne qui demande l’API peut aussi y ajouter son logo en petit.

Retrouvez la documentation complète sur https://searcharea.ddns.net/v1/searcharea/docs/
