# Definición del Producto Mínimo Viable (MVP)

Se trata de definir el [Producto Mínimo Viable (MVP)](https://es.wikipedia.org/wiki/Producto_viable_m%C3%ADnimo) que permita saber si nuestra solución es válida o incluso cancelar el proyecto en caso contrario.

> _NOTA: esto último es una opción. No debemos dejarnos manipular por la falacia del [Costo hundido](https://es.wikipedia.org/wiki/Costo_hundido)_

Una vez se tiene toda la pila priorizada (al nivel de detalle adecuado para empezar a implementar), se deben escoger los elementos que hay que incluir para el MVP. Cuanto más sistémico sea un producto más difícil será aislarlo (porque habrá mucha interdependencia entre distintas partes del producto). De esos elementos **hay que detectar los más críticos para empezar por ellos** (los elementos esenciales que debe tener la aplicación para alcanzar el objetivo a nivel mínimo). Por tanto la prioridad de todos los servicios de terceros o librerías que en principio no deben suponer un reto deben bajar de prioridad en el MVP y se debe afrontar primero los riesgos detectados pues serán los que marquen en mayor medida los cambios futuros que haya que realizar en **La Pila**.

> _NOTA: Un ejemplo es cómo se planificó la película **Bohemian Rapsody** y la escena de Wembley del concierto Live Aid_

<div class="containerVideo">
    <iframe allow="autoplay; encrypted-media" allowfullscreen="" class="video" frameborder="0" src="https://www.youtube.com/embed/6hE0CyWbKW4"></iframe>
</div>

Ejemplos típicos de partes que se pueden posponer es la securización y gestión de usuarios, la generación de informes, GUIs de administración que puedan ser sustituidas por archivos de configuración, conexiones que puedan simularse, etc...

![MVP correctamente elegido](/imgs/mvp.webp)

Se debe tener en cuenta que **el MVP debe cubrir todos los aspectos del producto aunque sea una porción del producto final** y no estar descompensado tocando sólo funcionalidades que no sean de aprovechamiento para validarse.

> _NOTA: Ver concepto [Vertical Slice](https://en.wikipedia.org/wiki/Vertical_slice). Incluso puede valer una simulación del producto final hecha con cualquier herramienta de prototipado si el proyecto lo aconseja._

Se ha ido creando una mentalidad que el desarrollo en una aplicación en tres capas debería ir en el sentido Datos > Backend > Frontend. Personalmente recomiendo hacerlo al revés:
1. Si se empieza por el frontend el cliente va a poder intervenir activamente desde el principio. Es la capa más cercana a la experiencia de usuario, lo cuál es una parte esencial en el desarrollo del producto (no caer en la tentación habitual de la Administración Pública donde se piensa _"como ésta va a ser la aplicación oficial, van a tener que usarla... les guste o no"_)
1. Una vez que nos queda clara la experiencia que tenemos que alcanzar, se conoce la interface entre front y back. Incluso con cambios en el futuro entre esas dos partes hay opciones como [GraphQL](https://es.wikipedia.org/wiki/GraphQL) que permitirán mantener interfaces robustas aunque cambien las implementaciones.
1. Con los recursos técnicos actuales como el [ORM](https://es.wikipedia.org/wiki/Asignaci%C3%B3n_objeto-relacional) o las BBDD [NoSQL](https://es.wikipedia.org/wiki/NoSQL), se pueden persistir los datos aún con cambios en el modelo de forma poco traumática.
1. La opción más completa sería añadir [desarrollo guiado por el comportamiento (Behavior-Driven Development - BDD)](https://es.wikipedia.org/wiki/Desarrollo_guiado_por_comportamiento) donde la parte de negocio pudiera marcar los criterios de aceptación mediante test hechos con tecnología como [Cucumber](https://cucumber.io/)