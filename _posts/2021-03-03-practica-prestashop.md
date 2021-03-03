---
layout: post
title:  "Práctica Prestashop"
date:   2021-03-03 11:56:40 -0600
categories: jekyll 
---
# Instalación de PrestaShop usando contenedores Docker y Docker Compose

1. Creamos una máquina en Amazon EC2

2. Instalamos Docker y Docker-compose en la máquina.

3. Modificamos el usuario.

        sudo usermod -aG docker $USER

4. Actualizamos el grupo docker.

        newgrp docker

5. Hacemos que docker sea un servicio que se inicie al arrancar la máquina.

        sudo systemctl enable docker

6. Iniciamos docker.

        sudo systemctl start docker

7. Creamos un docker-compose y un .env dentro de la carpeta prestashop

8. Realizamos un docker-compose up para realizar la instalación.

9. Accedemos a la IP pública de la instancia y procedemos a la instalación de prestashop.
