# Quiz App

Une application de quiz interactive développée avec Docker.

## Prérequis

- [Docker](https://www.docker.com/get-started) installé sur votre machine
- [Docker Compose](https://docs.docker.com/compose/install/) installé

## Installation

### 1. Configuration de l'environnement

Créez votre fichier de configuration d'environnement à partir du template fourni :

```bash
cp .env.example .env
```

Modifiez le fichier `.env` selon vos besoins si nécessaire.

### 2. Démarrage de l'application

Lancez l'application avec Docker Compose :

```bash
docker-compose up -d
```

L'option `-d` permet d'exécuter les conteneurs en arrière-plan (mode détaché).

## Accès à l'application

Une fois les conteneurs démarrés, l'application est accessible à l'adresse :

**http://localhost**

## Commandes utiles

### Voir les logs
```bash
docker-compose logs -f
```

### Arrêter l'application
```bash
docker-compose down
```

### Redémarrer l'application
```bash
docker-compose restart
```

### Reconstruire les conteneurs
```bash
docker-compose up -d --build
```

## Structure du projet

Consultez les fichiers suivants pour plus d'informations :
- `.env.example` : Variables d'environnement nécessaires
- `docker-compose.yml` : Configuration des services Docker

## Dépannage

Si vous rencontrez des problèmes :

1. Vérifiez que Docker est bien lancé
2. Assurez-vous que les ports nécessaires ne sont pas déjà utilisés
3. Consultez les logs avec `docker-compose logs`
4. Essayez de reconstruire les conteneurs avec `docker-compose up -d --build`
