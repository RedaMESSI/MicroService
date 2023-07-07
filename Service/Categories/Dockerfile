# Spécifie l'image de base
FROM node:14

# Définit le répertoire de travail dans le conteneur
WORKDIR /categories

# Copie les fichiers nécessaires dans le conteneur
COPY package.json package-lock.json /categories/

# Installe les dépendances
RUN npm install

# Copie le reste des fichiers dans le conteneur
COPY . /categories

# Expose le port sur lequel le serveur Express écoute
EXPOSE 3002

# Démarre le serveur Express
CMD ["node", "categories-service.js"]
