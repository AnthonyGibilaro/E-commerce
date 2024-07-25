# E-commerce :shopping_cart:

## Table des Matières

- [Introduction](#introduction)
- [Fonctionnalités](#fonctionnalités)
- [Prérequis](#prérequis)
- [Installation](#installation)
- [Utilisation](#utilisation)
- [Auteur](#auteur)

## Introduction

Le projet "E-commerce" est développé en utilisant le langage de programmation PHP et le framework Symfony pour le backend, et React.js pour le frontend. Il s'agit d'une plateforme de site marchand spécialisée dans les composants informatiques compatibles, offrant une expérience d'achat simplifiée et minimisant les retours de produits.

## Fonctionnalités

- **Gestion des utilisateurs** : Les utilisateurs peuvent créer un compte, se connecter, se déconnecter et gérer leurs informations personnelles. Les administrateurs ont des droits supplémentaires pour gérer les utilisateurs.
- **Catalogue de produits** : Affichage des articles avec descriptions, photos, caractéristiques et prix. Les utilisateurs peuvent trier les articles par nom, description, catégorie, etc.
- **Panier d'achat** : Les utilisateurs peuvent ajouter des articles à leur panier, visualiser et modifier le contenu de leur panier.
- **Commandes et livraisons** : Les utilisateurs peuvent passer des commandes, suivre leur statut, et gérer les informations de livraison. Les administrateurs peuvent gérer les frais de port et les commandes.
- **Administration** : Les administrateurs peuvent ajouter, modifier, supprimer des produits, gérer les stocks, les promotions, et les catégories.

## Prérequis

- PHP 7.3 ou supérieur
- Composer
- Node.js et npm
- XAMPP MySQL

## Installation

### Backend (Symfony)

1. Clonez le dépôt GitHub.

    ```sh
    git clone https://github.com/votre-repo/e-commerce.git
    ```

2. Allez dans le répertoire de l'API.

    ```sh
    cd api
    ```

3. Installez les dépendances PHP avec Composer.

    ```sh
    composer install
    ```

4. Créez une base de données MySQL en utilisant XAMPP.

5. Configurez votre fichier `.env` avec vos informations de base de données et les clés JWT.

    ```env
    DATABASE_URL="mysql://root:@127.0.0.1:3306/e-commerce"
    JWT_SECRET_KEY=%kernel.project_dir%/config/jwt/private.pem
    JWT_PUBLIC_KEY=%kernel.project_dir%/config/jwt/public.pem
    JWT_PASSPHRASE=yourpassphrase
    ```

6. Exécutez les migrations pour créer les tables dans votre base de données.

    ```sh
    php bin/console doctrine:migrations:migrate
    ```

7. Lier le stockage local.

    ```sh
    php bin/console assets:install
    ```

### Frontend (React)

1. Allez dans le répertoire du frontend.

    ```sh
    cd client
    ```

2. Installez les dépendances npm.

    ```sh
    npm install
    ```

## Utilisation

### Backend

1. Allez dans le répertoire de l'API.

    ```sh
    cd api
    ```

2. Lancez le serveur Symfony.

    ```sh
    symfony server:start
    ```

### Frontend

1. Allez dans le répertoire du frontend.

    ```sh
    cd client
    ```

2. Lancez le serveur de développement React.

    ```sh
    npm start
    ```

3. Accédez à l'interface utilisateur via votre navigateur à l'adresse `http://localhost:3000`.

## Auteur

👤 **Anthony GIBILARO**

* Site: [Portfolio](https://www.agibilaro.com/)
* GitHub: [@Github-GIBILARO-Anthony](https://github.com/Github-GIBILARO-Anthony)
* LinkedIn: [@Anthony Gibilaro](https://www.linkedin.com/in/anthony-gibilaro/)
