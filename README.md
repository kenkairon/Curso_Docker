# Curso_Docker
Curso Profesional de Docker

---
## Tabla de Contenidos
- [Docker](#Docker)
- [Caracteristicas Principales](#caracteristicas-principales)
- [Comandos de Docker](#comados-de-docker)
---
# Docker
- Docker es una plataforma de contenedorización que permite empaquetar aplicaciones y todas sus dependencias en un contenedor, asegurando que funcionen de manera consistente en cualquier entorno..
- 
--- 
# Caracteristicas Principales
1. Características principales de Docker
    ```bash 
    ✅Portabilidad: Los contenedores pueden ejecutarse en cualquier sistema que tenga Docker instalado (Windows, Linux, macOS, servidores en la nube, etc.).
    ✅ Aislamiento: Cada contenedor tiene su propio entorno (bibliotecas, variables de entorno, archivos de configuración, etc.), evitando conflictos entre aplicaciones.
    ✅ Ligereza: A diferencia de las máquinas virtuales, los contenedores comparten el mismo kernel del sistema operativo, por lo que consumen menos recursos.
    ✅ Escalabilidad: Facilita la implementación y gestión de múltiples instancias de una aplicación.

2. Conceptos clave de Docker
    ```bash 
    Imagen 📦: Es una plantilla inmutable con el sistema operativo, dependencias y la aplicación lista para ejecutarse.
    Contenedor 🚀: Es una instancia en ejecución de una imagen.
    Dockerfile 📜: Es un archivo con instrucciones para crear una imagen personalizada.
    Docker Hub 🌍: Un repositorio donde se almacenan y comparten imágenes de Docker.

# Comandos de Docker
3. Comandos docker Descargamos la Imagen 
    ```bash 
    docker pull httpd

4. Buscar una imagen en general
    ```bash
    docker image ls

5. Buscar una imagen en lo específico httpd
    ```bash
    docker image ls httpd

6. Ejecutar la imagen
    ```bash
    docker run -p 8080:80 httpd
        
7. Menu de ayuda de docker
    ```bash
    docker run --help

8. Contenedores Comandos Básicos menu
    ```bash
    docker container  --help

9. Buscamos que contiene los contenedores
    ```bash 
    docker container ls

10. Aplicamos run al test
    ```bash 
    docker run -p 8080:80 --name test nginx

11. Nos si situamos en otra terminal para ver la ejecución
    ```bash     
    docker container ls


12. Revisamos con inspect el test y nos va expresar un json
    ```bash 
    docker container inspect test  

13. Listamos todos los contenedores
    ```bash	
    docker container ls -a 

14. Para eliminar contenedores con el nombre
    ```bash
    docker container rm nostalgic_sinoussi

15. Para eliminar contenedores con el id
    ```bash
    docker container rm 79390d42eeda

16. Este elimina todos los contendores
    ```bash
    docker container prune
