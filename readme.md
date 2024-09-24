# Projet de Découverte d'API Platform

Ce projet est une application Symfony qui utilise API Platform pour gérer des entités `Membre` et interagir avec une API externe pour afficher et ajouter des utilisateurs.

## Prérequis

- PHP >= 7.4
- Composer
- Symfony CLI
- Node.js et npm (pour la gestion des dépendances front-end)

## Installation

1. Clonez le dépôt :

    ```bash
    git clone https://github.com/votre-utilisateur/votre-projet.git
    cd votre-projet
    ```

2. Installez les dépendances backend :

    ```bash
    composer install
    ```

3. Installez les dépendances front-end :

    ```bash
    npm install
    ```

4. Configurez votre base de données dans le fichier `.env` :

    ```dotenv
    DATABASE_URL="mysql://db_user:db_password@127.0.0.1:3306/db_name"
    ```

5. Créez la base de données et exécutez les migrations :

    ```bash
    php bin/console doctrine:database:create
    php bin/console doctrine:migrations:migrate
    ```

6. Démarrez le serveur Symfony :

    ```bash
    symfony server:start
    ```

## Utilisation

### Affichage des utilisateurs

Accédez à l'URL suivante pour voir la liste des utilisateurs :

http://localhost:8000/users

