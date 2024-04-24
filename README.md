# Aves de Chile
La asociación de Amantes de los pájaros de Chile ha notado que actualmente no se tiene información de los distintos pájaros que pueden ser observados en Chile. Es por eso que les gustaría poder entender a manera de prototipo cómo listar muchos de estos especímenes. Para ello se les solicita generar un prototipo muy sencillo en el cual se puedan observar algunas imágenes de pájaros típicos de Chile junto con su nombre en español e inglés. La idea es que esta información pueda ser eventualmente transformada en señaléticas bilingües que permitan fomentar el turismo en Chile.

## Se ha desarrollado un script en Python que cumple con los requerimientos solicitados. A continuación se describen los pasos seguidos:

## 1. Crear templates del HTML a utilizar
Se han creado los siguientes templates:

## base.html: Template base que define la estructura general de la página.
## bird.html: Template que muestra la información de cada especie de pájaro.
## 2. Generar un llamado a la API que permita recopilar la información necesaria
Se ha utilizado la API 'https://aves.ninjas.cl/api/birds' para obtener la información requerida. Se ha implementado un módulo llamado bird_info.py que realiza la llamada a la API y procesa los datos necesarios para la construcción del sitio web.

## 3. Exportar el sitio creado como un archivo HTML que pueda ser abierto en el navegador
Se ha implementado un script llamado generate_site.py que utiliza los templates HTML y la información obtenida de la API para generar un archivo HTML (index.html) que puede ser abierto en el navegador.

## Ejecución del Script
Para ejecutar el script y generar el sitio web, sigue estos pasos:

## bash
Copy code
python generate_site.py
Esto generará un archivo index.html en el directorio actual. Abre este archivo en tu navegador para ver el sitio web generado con la información de las aves de Chile.

## Estructura del Proyecto
csharp
Copy code
.
├── templates
│   ├── base.html
│   └── bird.html
├── bird_info.py
├── generate_site.py
└── README.md
## templates: Directorio que contiene los templates HTML.
## bird_info.py: Módulo Python que realiza la llamada a la API y procesa la información de las aves.
## generate_site.py: Script principal que genera el sitio web.
README.md: Este archivo, que proporciona información sobre el proyecto y su ejecución.
## Nota
A pesar de que el requerimiento es sencillo, se han respetado las buenas prácticas de modularización para garantizar la mantenibilidad y escalabilidad del código.
---------------------------------------------------------------------------------------------------------------------------------------------
¡Gracias por revisar mis proyectos! Si tienes alguna pregunta o sugerencia, no dudes en contactarme.
