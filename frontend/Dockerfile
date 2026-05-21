FROM node:22-alpine

# Définir le dossier de travail
WORKDIR /app

# Copier les fichiers de package
COPY package*.json ./

# Installer les dépendances
RUN npm install

# Copier le reste du code
COPY . .

# Exposer le port de développement de Vite (par défaut 5173, souvent exposé sur ce port)
EXPOSE 5173

# Commande pour démarrer Vite en mode développement
CMD ["npm", "run", "dev", "--", "--host"]
