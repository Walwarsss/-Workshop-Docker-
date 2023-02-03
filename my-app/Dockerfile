# Utiliser une image Node.js officielle en tant qu'image de base
FROM node:14

# Définir le répertoire de travail
WORKDIR /app

# Copier les fichiers package.json et package-lock.json
COPY package*.json ./

# Installer les dépendances de l'application
RUN npm install

# Copier le reste du code source de l'application
COPY . .

# Spécifier la commande à exécuter lorsque le conteneur démarre
CMD [ "npm", "start" ]

# Exposer le port de l'application
EXPOSE 3000
