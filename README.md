# 💪 Challenge
"The Cookie Factory" lance son site e-commerce
À partir des ressources ci-dessus et du template que tu peux récupérer sur github tu vas pouvoir commencer le développement du site e-commerce : "The Cookie Factory"

Il s'agit d'une petite application qui permet de s'identifier avec seulement un nom d'utilisateur, sans appel à une base de données.

On entre un nom d'utilisateur dans le formulaire de login. Celui-ci est pris en compte et enregistré en session. On ne demande pas de mot de passe pour vérifier l'identité.

Si l'utilisateur n'est pas identifié, il n'a pas accès aux pages du site internet autres que login.php et index.php.

Tant qu'il n’y a pas de variable de session contenant le nom de l'utilisateur, celui-ci est redirigé vers la page de login. Tu peux chercher sur ton moteur de recherche favori comment rediriger en PHP.

Une fois identifié, l'utilisateur est redirigé sur la page index.php où l'on trouve la liste des produits disponibles. Et bien évidemment, il n'est plus possible d’accéder à la page de login. Petite astuce ;)

Sur cette page, toute une liste de biscuits s'offre à toi. Lorsqu'un client clique sur le bouton d'ajout au panier, il faut enregistrer cet article dans tes données de session.

Libre à toi de modifier le comportement du bouton pour que l'ajout soit pris en compte.
Avant d’enregistrer dans $_SESSION le panier du client, tu auras peut-être besoin de faire transiter l'information via $_GET ou $_POST.
Tu n’es pas obligé de gérer les quantités pour chaque élément afin de réussir cette quête.

Comme tu peux le voir, dans la barre de menu, on souhaite la bienvenue à "Wilder". Sers-toi du nom de l'utilisateur pour personnaliser le message d'accueil.

Si un utilisateur souhaite se déconnecter de la page, il peut cliquer sur le bouton “Se déconnecter” (visible uniquement lorsque l’utilisateur est connecté). Ce qui aura pour effet de détruire la session en cours ainsi que toutes les informations.

Critères de validation
On peut s'identifier de manière simple avec seulement un nom d'utilisateur,
Le nom d'utilisateur, donné lors de l'identification, est affiché dans le header sur toutes les pages à partir des informations de sessions,
Le panier est stocké dans la session de l’utilisateur et est affiché sur la page "Panier".
Il est possible d’accéder uniquement aux pages login.php et index.php tant que l’utilisateur n’est pas connecté.
La page login.php devient inaccessible une fois l’utilisateur connecté. Ce dernier est redirigé vers la page index.php s'il tente d'y accéder.
L'utilisateur peut également se délogger à l'aide d'un bouton "déconnexion" et la session est alors détruite.
[BONUS] Gérer les quantités de cookies dans ton panier. Cette tâche est assez complexe, tu peux tenter de le faire, mais ce n’est pas le but de la quête. Ne perds pas plus de temps que de raison là-dessus.
