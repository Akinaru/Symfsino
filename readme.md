# README — Plateforme de jeux (Symfony)

## Tutoriel
_Un tutoriel pas-à-pas arrive bientôt._  
Il couvrira : installation locale, configuration `.env`, création BDD, lancement du serveur et premiers écrans.

## Objectifs d’apprentissage
- Maîtriser le cycle complet d’une application Symfony : conception → développement → tests → déploiement local.
- Utiliser de façon cohérente les piliers du framework : Security, Forms, Validator et Doctrine.
- Structurer un domaine métier clair : comptes, jetons, parties, mises et gains.
- Concevoir une architecture extensible facilitant l’ajout de nouveaux jeux.
- Isoler la logique de jeu dans des services testables (moteur, RNG, calculs).
- Mettre en place une observabilité minimale (logs, événements, métriques simples).
- Établir un aspect communautaire via un serveur WebSocket permettant aux joueurs de jouer et de communiquer entre eux.

## Roadmap (grandes étapes)
- Setup projet Symfony propre : arborescence, env (`.env`/`.env.local`), base de données.
- Authentification/inscription : création de compte, login, vérif e-mail, reset password, protections CSRF/rate-limit.
- Module Profil : vue/édition du profil (pseudo, avatar, préférences), page profil public minimal.
- Design system / UI de base : layout, thèmes, composants réutilisables (boutons, listes, formulaires).
- Noyau “moteur de jeu” : entités génériques (Session, Player, Round, Event, Score) + interface `GameTemplate` pour plugger des jeux.
- Panneau Admin minimal : gestions des utilisateurs (monnaie, statistiques).
- Implémentation du Jeu #1.
- Implémentation du Jeu #2.
- Temps réel avec Mercure : chat en direct, leaderboard, action en direct (envoie de monnaie).
- Statistiques & profil enrichi : historique de parties, meilleurs scores, badges/récompenses simples.
