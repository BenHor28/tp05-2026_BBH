## Démarrer le projet

Exécutez ces commandes depuis le dossier du projet.

### Initialiser et lancer Terraform

```bash
terraform init   #Télécharge et installe le provider Docker configuré dans main.tf
terraform plan   #Vérifie la liste des ressources que Terraform va créer
terraform apply  #Lance la création du réseau, la construction des images et le démarrage des conteneurs
```

Confirmez l’application avec `yes` si demandé.

### Construire et démarrer les conteneurs Docker

```bash
docker compose up --build -d
```

Pour arrêter les conteneurs :

```bash
docker compose down
```

### Ouvrir le site web

Dans votre navigateur, ouvrez `http://localhost:8080`. Remplacez `8080` par le port indiqué dans la configuration Docker Compose si nécessaire.
