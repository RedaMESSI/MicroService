# Spécifie l'image de base
FROM node:14

# Définit le répertoire de travail dans le conteneur
WORKDIR /books

# Copie les fichiers nécessaires dans le conteneur
COPY package.json package-lock.json /books/

# Installe les dépendances
RUN npm install

# Copie le reste des fichiers dans le conteneur
COPY . /books

# Expose le port sur lequel le serveur Express écoute
EXPOSE 3000

# Démarre le serveur Express
CMD ["node", "books-service.js"]