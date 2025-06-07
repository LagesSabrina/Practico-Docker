
# Práctico: Git + Docker

Proyecto simple que sirve una página HTML estática usando un contenedor Docker con la imagen oficial de NGINX.

## Contenido

- `index.html`: página HTML simple que se sirve con NGINX.

## Pasos realizados


1. **Creacion del proyecto**

   - Cree la carpeta `Practico-Docker`.
   - Dentro de esta carpeta cree un archivo `index.html` con contenido HTML.

2. **Descarga de la imagen oficial de NGINX**

   Ejecute en la terminal:
   docker pull nginx

3. **Ejecucion del contenedor Docker**

    Desde dentro de la carpeta Practico-Docker, corri el siguiente comando:
    docker run -d -p 8080:80 -v ${PWD}:/usr/share/nginx/html nginx

3. **Verificacion**
 
    Abrí el navegador y entré a http://localhost:8080, donde se mostro la pagina HTML.

3. **Verificacion 2**
  
    Verificar si mi contenedor esta corriendo con este comando:
    docker ps