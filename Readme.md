# Squelette de projet
## Context
Dans le cadre de notre séance de formation, nous avons implémenté cette architecture projet.

## Container Docker

- php-fpm
- nginx
- postgreSql

## Projet

- symfony 6.*

## Dev tools
- symfony phpunit-bridge
- php-cs-fixer
- phpstan

### Objectif du make install
- installer les dépendances => composer install
- copier les variables d'environnement de database.env dans le .env
- copier dans le symfony/config/packages/doctrine.yml la configuration postgresql
- lancer les container => make start