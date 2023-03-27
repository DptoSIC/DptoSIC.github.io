# Burndown

Para conocer si el ritmo que llevamos es suficiente para alcanzar el Sprint Goal se utiliza el [Diagrama Burndown](https://es.wikipedia.org/wiki/Burn_down_chart) (hay más herramientas para ello, pero nos vamos a centrar en el Burndown por su sencillez y uso habitual). En resumen es plasmar en un gráfico dos líneas:
1. una guía que representa un ritmo constante de trabajo finalizado hasta justo completar el `Sprint Backlog` dentro de la duración del Sprint (línea recta discontinua de la figura)
2. una línea quebrada que refleja el progreso del trabajo realizado conforme se modifica el estado de los elementos del `Sprint Backlog` (línea verde)

La [versión premium del GitLab incluye un complemento llamado Burndown Chart](https://docs.gitlab.com/ee/user/project/milestones/burndown_and_burnup_charts.html) que lo dibuja como la siguiente figura: 

![Ejemplo Burndown](https://docs.gitlab.com/ee/user/project/milestones/img/burndown_chart_legacy_v13_6.png)

Para nuestro repositorio GitEIE se ha implementado un [diagrama Burndown personalizado](https://burndown-dim.netlify.app/) utilizando la magnífica [API de GitLab](https://docs.gitlab.com/ee/api/issues.html). Puedes ver cómo utilizarlo en su [demostración en vídeo](https://youtu.be/_krAgjeZrI4).

Este es un ejemplo del Sprint 2 del proyecto InfraStruturas:

![Ejemplo Burndown Combat Agile Tools](/imgs/burndown-combat-agile.webp)

Idealmente debería haber cierres todos los días (en la Daily o cierre del día anterior).

En este caso se ven algunos cierres numerosos a la vez. Esto puede deberse a que al "Merge" de una rama que acumula varios "Fixes". El diagrama refleja los commits que llegan a la rama master, no los que haya en otras ramas pero si formar parte aún del incremento.