# PARTICIPANTES:
#    Neil Aular
#    Francisco Jara
#    Francisco Vargas
#    Jorge Riquelme
#    Diego Jimenez
#    Fernando Poblete

# Task API Project
Este proyecto demuestra una API sencilla, integrada con contenedores DOCKER, y enlazado con Jenkins para la integracion CI/CD 

## Features

Tiene 2 endpoint sencillos:  /tasks  y 
-  /tasks  : Lista todas las tareas
-  /tasks/:id   : Consulta tarea por ID

## Running Locally

1. Instalar dependencias: `npm install express`  
2. Inicio del servidor: `npm start app`

## Running with Docker

1. Genera la imagen: `docker build -t desafio08 desafio08grupo02:latest .`  
2. Ejecuta el contenedor: `docker run -p 3000:3000 –name desafio08 desafio08grupo02:latest`

