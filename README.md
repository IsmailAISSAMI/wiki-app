# Rails Wikipedia

Le but du projet est de créer un site similaire à Wikipédia avec quelques fonctionnalités supplémentaires. À l’issue du projet, le rendu se composera du code (un dépôt GitHub) ainsi que d’un rapport de moins de 5 à 10 pages détaillant ce que vous avez fait, comment vous vous y êtes pris, et comment vous pourriez faire évoluer le projet.

Le projet peut se réaliser individuellement, ou en groupe de 2 à 3 personnes. Le rendu se fera au plus tard le dimanche 20/12/2020 à 23:59.

Le projet est en deux parties : la partie requise, et la partie bonus. Il faut se concentrer sur la partie requise, qui doit fonctionner. Vous êtes ensuite libres d’implémenter une ou plusieurs fonctionnalités bonus si vous le souhaitez.

# Requis

Pour le projet, il est nécessaire de partir d’un nouveau projet à l’aide d’un `rails new`. Les ajouts de fonctionnalités se feront sur le projet uniquement. Héberger directement votre code sur GitHub, et commitez régulièrement (une fonctionnalité, un commit).

1. On souhaite ajouter la gestion des utilisateurs pour authentifier des individus. Un utilisateur doit avoir un username, un email, un mot de passe sécurisé. Le username ne doit pas pouvoir être modifié une fois créé.
2. On souhaite ajouter la gestion des articles à l’application. Un article se compose d’un auteur (utilisateur) et d’un contenu (string).
    - Commencez par créer le modèle et le controlleur.
    - Ajouter une page pour créer un article.
    - Ajouter une page pour modifier un article.
3. À chaque modification d’un article, on souhaite garder les révisions précédentes pour les comparer. Proposez une solution pour garder l’historique des révisions d’un article.
4. On souhaite envoyer une notification par email à chaque fois qu’une révision a lieu sur un article que l’on a soi-même édité par le passé.
    - Créez un mailer pour envoyer un mail
    - À chaque modification d’article, vérifiez à quel utilisateur il faut envoyer un mail.
7. On souhaite faire un classement des utilisateurs par point en créant un système de rangs. Chaque utilisateur commence avec un solde de points vides (0 points) et gagne des points pour chaque action sur le site. Proposez un système pour conserver les points. Les points se décomptent comme suit : 1 article créé = 1 point, 1 article édité = 0.5 points. Décomptez les points par utilisateur puis créez une page pour afficher les tops utilisateurs.

# Bonus

- Ajouter la gestion des images dans le corps du texte.
- Ajouter la gestion des mentions dans le corps du texte.
- Créer un système de commentaires pour chaque publication.
- Ajouter la gestion du contenu des pages en Markdown pour faciliter l’édition.
- Créer un système de brouillon. Chacun pourra commencer un article et le sauvegarder sur son compte pour le retrouver plus tard.
- Créer un système de modération : avant chaque publication / modification, l’aval doit être donné par un membre ayant plus de 100 points (ou un administrateur).
- Détecter les liens interpages et les afficher dans une section en bas de la page ou directement dans la page, au choix.
