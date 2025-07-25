# Reto Articulos MELI

Reto por Felix Antonio Sirit Murillo siritfelix@gmail.com

Tecnologías necesarias

`Java 21` `Maven` `Spring-Boot 3.5` `h2` `liquibase` `JPA` `Angular - 18`

Instalación del proyecto

Pasos para levantar la aplicacion:
1) Clonar el proyecto con 
    > git clone https://github.com/siritfelix/article-back-front.git

2) Como el proyecto contiene 2 Submodulos de git es necesario que se descargen el modulo de backend y el frontend
    > cd article-back-front

    > git submodule update --init --recursive

3) Instalacion con docker, el proyecto tiene un archivo docker-compose.yml para crear 2 contenedores uno para el back y otro para el front, con el siguiente comando se construyen las imagenes y se levantan
    
    > docker-compose up -d --build

4) El servicio de frontend queda desplegado en http://localhost:4200/article

5) La documentacion de la api se puede visualizar en http://localhost:8080/v1/swagger-ui/index.html