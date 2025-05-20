# Helpdesk - Système de gestion de tickets d'assistance

Ce projet est une application PHP permettant aux utilisateurs de soumettre des demandes d’assistance (tickets), et aux techniciens de les consulter et de les traiter via une interface sécurisée.

## Objectif

Mettre en place un système d’assistance simple, avec deux interfaces :
- Une interface pour les utilisateurs afin de créer des tickets.
- Une interface pour les techniciens afin de consulter et gérer les tickets.

## Fonctionnalités développées

### Page d’accueil
- Page d’introduction au service d’assistance.
- Lien vers la page de demande d’assistance.

### Création de tickets (utilisateur)
- Formulaire de création d’un ticket.
- L’utilisateur saisit des informations comme : nom, email, sujet, description.
- Un numéro de ticket unique est généré automatiquement.
- Le ticket est enregistré avec le statut "ouvert".

### Interface technicien (accès sécurisé)
- Accès protégé par `.htaccess` / `.htpasswd`, réservé aux techniciens.
- Affichage de la liste des tickets avec leur statut :
  - Ouvert
  - En cours
  - Fermé
- Détail de chaque ticket consultable individuellement.
- Possibilité de mettre à jour le statut d’un ticket.

## Sécurité

- L’accès à l’espace technicien est protégé via une authentification HTTP.
- L’interface utilisateur reste accessible sans authentification.

## Technologies utilisées

- Langage : PHP
- Sécurité : `.htaccess` / `.htpasswd` pour l’authentification
- Stockage : (ajouter ici si vous utilisez une base de données ou un système de fichiers)

## Partie du projet non faites 
- panneau d'accueil présentant les tickets avec leur statu ( avec couleur selon le statut)
- page de consultation des tickets
- mise en place de fonctionnalités que vous trouverez utile
- utilisation de css