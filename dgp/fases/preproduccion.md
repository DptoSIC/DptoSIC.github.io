# Preproducción

Para la implementación se usará [_"Combat Agile"_](/dgp/combat-agile/indice) (aunque también se puede usar desde el concepto).

La fase de preproducción se enfoca a realizar el MVP con un equipo de desarrollo reducido. Persigue validar la solución propuesta y minimizar el empleo de recursos en caso contrario.

![Scrum vs Tradicional](/imgs/scrum-vs-tradicional.webp)

En general las prácticas del curso se ciñen a esta fase de preproducción, ya que no es normal que por plazos de tiempo se pueda llegar a producción o se amplíe el equipo con personal de la UCO. **Nuestro objetivo de producto general será proporcionar un MVP que sirva de prototipo a la UCO** para que, en caso de ser aprobado por la Autoridad correspondiente, pueda continuar la producción y mantenimiento con su propio personal.

> No obstante, desplegar en la red corporativa usando la infraestructura aprobada oficialmente es lo recomendable, aunque por el escaso tiempo para obtener la autorización no es un escenario realista de manera general.

Habitualmente el entorno de desarrollo/pruebas será Internet usando servicios como:
1. [GitEIE](https://git.institutomilitar.com/)/[GitHub](https://github.com/) para control de versiones, repositorio de documentación (wikis) y gestión de tareas (kanbans)
1. [Heroku](https://www.heroku.com/) para el servidor de aplicaciones
1. [Netlify](https://docs.netlify.com/) para el servidor web
1. [ElephantSQL](https://www.elephantsql.com/) o Heroku como BD en la nube

Este entorno se observa en el siguiente diagrama:

![Arquitectura DevOps](/imgs/devops.webp)

El uso de este entorno se incluye en esta asignatura y está [explicado en vídeo](https://youtu.be/Qd9PhRKPhEs).
