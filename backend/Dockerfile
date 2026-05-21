FROM node:22-alpine

# Définir le dossier de travail
WORKDIR /app

# Copier les fichiers de package
COPY package*.json ./

# Installer les dépendances
RUN npm install

# Copier le reste du code
COPY . .

# Exposer le port
EXPOSE 3000

# Commande pour démarrer l'application
CMD ["node", "index.js"]
