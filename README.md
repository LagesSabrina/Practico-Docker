
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

4. **Uso de Git y GitHub**

   Inicialice un repositorio en la carpeta del proyecto:
    git init

   Configure mi usuario de Git:
    git config --global user.name "Mi Nombre"
    git config --global user.email "miemail@istea.com"
   
   Agregue todos los archivos al repositorio local:
    git add .

   Hice el primer commit:
    git commit -m "Primer commit"

   En GitHub, cree un repositorio vacio llamado Practico-Docker.
   Vincule mi repo local con el de GitHub:
    git remote add origin https://github.com/miusuario/Practico-Docker.git

   Subí todo al repositorio remoto:
    git branch -M main
    git push -u origin main