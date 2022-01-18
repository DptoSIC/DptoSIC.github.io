# Definición del Producto Mínimo Viable (MVP)

Aquí se trata de definir el [Producto Mínimo Viable (MVP)](https://es.wikipedia.org/wiki/Producto_viable_m%C3%ADnimo) que permita saber si nuestra solución es válida o incluso cancelar el proyecto en caso contrario.

Una vez se tiene toda la pila priorizada (al nivel de detalle adecuado para empezar a implementar), se deben escoger los elementos que hay que incluir para el MVP. Cuanto más sistémico sea un producto más difícil será aislarlo (porque habrá mucha interdependencia entre distintas partes del producto). De esos elementos **hay que detectar los más críticos para empezar por ellos** (los elementos que si no se pueden realizar la aplicación no tiene negocio). Por tanto la prioridad de todos los servicios de terceros o librerías que en principio no deben suponer un reto deben bajar de prioridad en el MVP y se debe afrontar primero los riesgos detectados pues serán los que marquen en mayor medida los cambios futuros que haya que realizar en **La Pila**.

Ejemplos típicos de partes que se pueden posponer es la securización y gestión de usuarios, la generación de informes, GUIs de administración que puedan ser sustituidas por archivos de configuración, conexiones que puedan simularse, etc...

![MVP correctamente elegido](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fbrianpagan.net%2Fwp-content%2Fuploads%2F2015%2F08%2FMVP-brianpagan.net-diagram1.png&f=1&nofb=1)

Se debe tener en cuenta que **el MVP debe cubrir todos los aspectos del producto aunque sea una porción del producto final** y no estar descompensado tocando sólo funcionalidades que no sean de aprovechamiento para validarse.

> _NOTA: Ver concepto [Vertical Slice](https://en.wikipedia.org/wiki/Vertical_slice). Incluso puede valer una simulación del producto final hecha con cualquier herramienta de prototipado si el proyecto lo aconseja._
