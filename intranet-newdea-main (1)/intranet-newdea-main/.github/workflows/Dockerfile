# Image de base nginx alpine 3.23
FROM nginx:alpine3.23
# par :
FROM nginx:alpine3.23-slim

# Supprimer la page par défaut de nginx
RUN rm -rf /usr/share/nginx/html/*

# Copier les fichiers du site statique
COPY . /usr/share/nginx/html/

# Exposer le port 80
EXPOSE 80

# Lancer nginx
CMD ["nginx", "-g", "daemon off;"]