#Extraction d'une image de base ici node 6
FROM node:6
# Creation du repertoire de travail de l'application
WORKDIR /usr/src/app
#copie de toutes les fichiers json vers le repertoire de travail
COPY package*.json ./
#nettoyage du cache
RUN npm cache clean
#Installation des dépendences
RUN npm install
# source d'application
COPY . .
#le port vue de l'exterieur
Expose 3000
# Execute le code pour le lancement de l'application
CMD ["node","index.js"]
