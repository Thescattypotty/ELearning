# Cahier des Charges pour une Plateforme d'Apprentissage en Ligne

## 1. Introduction
### Objectif du projet:


Créer une plateforme d'apprentissage en ligne permettant aux utilisateurs de s'inscrire, de s'abonner à des cours, et d'accéder à des ressources pédagogiques. La plateforme doit offrir une interface conviviale pour les étudiants, les instructeurs et les administrateurs.

## 2. Fonctionnalités Principales:

### 2.1 Authentification et Autorisation:

- Inscription et connexion des utilisateurs
- Rôles d'utilisateur (Administrateur, Instructeur, Étudiant)
- Gestion des permissions basées sur les rôles

### 2.2 Gestion des Cours:

- Création, modification et suppression de cours par les instructeurs
- Approbation des cours par les administrateurs
- Inscription des étudiants aux cours

### 2.3 Livraison de Contenu:

- Modules de cours avec texte, vidéo et quiz
- Téléchargement de ressources

### 2.4 Interaction:

- Forums de discussion pour chaque cours
- Messagerie directe entre étudiants et instructeurs

### 2.5 Suivi de Progression:

- Suivi de la progression des étudiants et résultats des quiz
- Génération de certificats à la fin des cours

### 2.6 Gestion Administrative:

- Gestion des utilisateurs (CRUD)
- Vue d'ensemble des statistiques de la plateforme

## 3. Technologies Utilisées:
- Backend: Symfony (PHP)
- Frontend: HTML, CSS, JavaScript (avec Twig pour le templating côté serveur)
- Base de Données: Sqlite
- Sécurité: Symfony Security Bundle

## 3. Guide d'installation : 
### Requirements : 

| Tech | Requirements | 
| :---- | :------------: |
| OS | Linux (Debien recommandé), macOS, ou Windows |
| Server Web | Apache ou Nginx |
| PHP | PHP 8.1 ou supérieur (Symfony **7** requiert PHP **8.1+**) |
| Database | SQLite **3.20+** |
| Gestionnaire de Packages | Composer |
| Outils de Développement | Git(optionel) |

### Guide de lancement du project :
1. Installation des prerequis : 
    `composer install`
2. Creation de la base de donnèes:
    `symfony console d:d:c`
3. Migration :
    `symfony console m:m`
    `symfony console d:m:m`        
4. Run Project : 
    `symfony server:start`    

> [!NOTE]
> If you don't have symfony cli : change commande `symfony console` by `php bin/console`