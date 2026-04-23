cat > Dockerfile << 'EOF'
FROM nginx:alpine

# Copiar el archivo HTML
COPY index.html /usr/share/nginx/html/index.html

# Crear un index.html por defecto si no existe
RUN echo "<h1>Bienvenido a OpenShift</h1>" > /usr/share/nginx/html/default.html

# Exponer el puerto 80
EXPOSE 80

# Iniciar nginx
CMD ["nginx", "-g", "daemon off;"]
EOF