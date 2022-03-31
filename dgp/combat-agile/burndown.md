# Burndown

Para conocer si el ritmo que llevamos es suficiente para alcanzar el Sprint Goal se utiliza el [Diagrama Burndown](https://es.wikipedia.org/wiki/Burn_down_chart) (hay más herramientas para ello, pero nos vamos a centrar en el Burndown por su sencillez y uso habitual). En resumen es plasmar en un gráfico dos líneas:
1. una guía que representa un ritmo constante de trabajo finalizado hasta justo completar el `Sprint Backlog` dentro de la duración del Sprint (línea recta discontinua de la figura)
2. una línea quebrada que refleja el progreso del trabajo realizado conforme se modifica el estado de los elementos del `Sprint Backlog` (línea verde)

La [versión premium del GitLab incluye un complemento llamado Burndown Chart](https://docs.gitlab.com/ee/user/project/milestones/burndown_and_burnup_charts.html) que lo dibuja como la siguiente figura: 

![Ejemplo Burndown](https://docs.gitlab.com/ee/user/project/milestones/img/burndown_chart_v13_6.png)

Para nuestro repositorio GitEIE se ha implementado un [diagrama Burndown personalizado](https://burndown-dim.netlify.app/) utilizando la magnífica [API de GitLab](https://docs.gitlab.com/ee/api/issues.html). Puedes ver cómo utilizarlo en su [demostración en vídeo](https://youtu.be/_krAgjeZrI4).