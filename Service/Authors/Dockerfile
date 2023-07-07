# Spécifie l'image de base
FROM node:14

# Définit le répertoire de travail dans le conteneur
WORKDIR /authors

# Copie les fichiers nécessaires dans le conteneur
COPY package.json package-lock.json /authors/

# Installe les dépendances
RUN npm install

# Copie le reste des fichiers dans le conteneur
COPY . /authors

# Expose le port sur lequel le serveur Express écoute
EXPOSE 3001

# Démarre le serveur Express
CMD ["node", "authors-service.js"]
