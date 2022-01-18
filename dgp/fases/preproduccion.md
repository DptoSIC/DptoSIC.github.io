# Preproducción

Para la implementación se usará como base los artefactos, roles y eventos de [Scrum](https://www.scrumguides.org/docs/scrumguide/v2020/2020-Scrum-Guide-Spanish-European.pdf). El uso y conocimiento de Scrum nos va a servir para poder trabajar con otro personal colaborador ya que es la referencia principal como forma de trabajo. Para entender la forma de trabajo ver el siguiente documento dedicado a ello Scrum.

La fase de preproducción se enfoca a realizar el MVP con un equipo de desarrollo reducido. Persigue validar la solución propuesta y minimizar el empleo de recursos en caso contrario.

![Scrum vs Tradicional](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fi.pinimg.com%2F736x%2F41%2Fd9%2Fa4%2F41d9a491ccbf82833e1a71accedfbafb--scrum-nice-people.jpg&f=1&nofb=1)

En general las prácticas del curso se ciñen a esta fase de preproducción, ya que no es normal que por plazos de tiempo se pueda llegar a producción o se amplíe el ED con personal de la UCO. Nuestro objetivo debe ser proporcionar un MVP que sirva de prototipo a la UCO para que en caso de ser aprobado pueda continuar con su producción y mantenimiento con su propio personal.

Habitualmente el entorno de desarrollo/pruebas será Internet usando servicios como:
1. [GitEIE](https://git.institutomilitar.com/)/[GitHub](https://github.com/) para control de versiones, repositorio de documentación (wikis) y gestión de tareas (kanbans)
1. [Heroku](https://www.heroku.com/) para el servidor de aplicaciones
1. [Netlify](https://docs.netlify.com/) para el servidor web
1. [ElephantSQL](https://www.elephantsql.com/) o Heroku como BD en la nube

Este entorno se observa en el siguiente diagrama:

![Arquitectura DevOps](imgs/devops.png)

El uso de este entorno se incluye en esta asignatura y está [explicado en vídeo](https://youtu.be/Qd9PhRKPhEs).

No obstante, desplegar en la red corporativa usando la infraestructura aprobada oficialmente es lo recomendable, aunque por el escaso tiempo para obtener la autorización no es un escenario realista de manera general.
