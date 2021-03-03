# desigom.github.io

# Creación de blogs con Jekyll y GitHub Pages

- Para consultar todos los comandos que podemos ejecutar con jekyll podemos ejecutar el siguiente comando:
        
        docker run -it --rm -v "$PWD:/srv/jekyll" jekyll/jekyll jekyll

- Este comando nos permite crear la estructura de directorios y los archivos necesarios de un nuevo proyecto Jekyll.

        docker run -it --rm -v "$PWD:/srv/jekyll" jekyll/jekyll jekyll new blog

- Este comando nos permite generar un sitio HTML estático a partir del contenido del proyecto Jekyll.

        docker run -it --rm -v "$PWD:/srv/jekyll" jekyll/jekyll jekyll build

    - Nota: Tenga en cuenta que este comando tendrá que ejecutarlo dentro del directorio donde tenga el contenido del blog.

- Este comando nos permite servir de forma local un sitio HTML estático generado a partir del contenido del proyecto Jekyll.

        docker run -it --rm -p 4000:4000 -v "$PWD:/srv/jekyll" jekyll/jekyll jekyll serve --force_polling

    - Nota: Tenga en cuenta que este comando tendrá que ejecutarlo dentro del directorio donde tenga el contenido del blog.

- Para ver nuestro sitio web sólo tenemos que abrir un navegador web y acceder a la dirección de localhost en el puerto 4000.

# Publicar una web estática en GitHub Pages

- Creamos un repositorio nuevo.

        desigom/desigom.github.io

- Subimos todos los archivos que se nos han creado anteriormente.
