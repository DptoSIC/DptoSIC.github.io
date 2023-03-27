# Seguimiento del Sprint

Una vez que tenemos nuestro Sprint Planning hecho llega el momento de hacer el seguimiento. La Daily es el momento para actualizar la situación. Abriendo nuestro tablero podemos ver cómo está la situación de los elementos de **La Pila**. Idealmente, al terminar la jornada laboral debemos haber hecho push de los commits que cumplan con la tarea que nos comprometimos en la Daily:
1. En cada Daily me asigno un elemento. Si no ha habido ningún cambio respecto al día anterior y **La Pila** está correctamente ordenada, deberían seleccionarse aquellas tareas que estén en lo más alto.
1. Cuando termino un elemento lo paso a la columna de completado. Esta es nuestra vista del `Sprint Backlog`:
    ![Vista hito sprint 1](/imgs/sprint1.png)
1. Lo mejor es que si un commit supera los criterios de aceptación de un issue añadamos al final del mensaje `Fix #??` (donde `#??` es el identificador del issue completado). De esta forma nuestra ficha de tarea se actualiza automáticamente (se cierra y contiene un enlace entre el commit y el issue).
1. El commit se hará sobre la rama apropiada (crear una rama para el issue/`PBI`s cuando corresponda), no directamente en master. **En master estará el incremento**.
1. Para que un `PBI` alcance la **`DoD`** se debe hacer merge sobre master para añadir el valor al incremento y desplegar en el entorno que corresponda.
    > _NOTA: ver [Trunk Based Development](https://trunkbaseddevelopment.com/) para clarificar los dos últimos puntos._
1. Es importante añadir comentarios de valor en los issues para futuras consultas (también adjuntar cualquier archivo relevante como por ejemplo el resultado de un test) y así mantendremos, de forma natural, una documentación con un contexto adecuado (cualquiera podrá saber qué se hizo y por qué examinando el historial y los comentarios).
1. Si no tengo tarea asignada cogeré otra o ayudaré a un compañero.
1. GitLab es capaz de mantener actualizados todos nuestros artefactos:
    ![Vista tablero automatizado](/imgs/tablero-sprint1.png)
1. Es recomendable visualizar el estado del diagrama [burndown](burndown) al empezar la Daily para conocer la situación del trabajo realizado y el pendiente.

En este momento podremos ver nuestro issue cerrado y en la columna correspondiente.

El esfuerzo de **cada elemento se puede estimar en GitLab utilizando la acción [`/estimate`](https://docs.gitlab.com/ee/user/project/time_tracking.html)**. Con la suma de las estimaciones de todos los issues del milestone podremos calcular el esfuerzo del milestone (que debería coincidir con la duración del Sprint).

Por todo ello **es fundamental tener claro** el tablero de la última figura para saber en qué estoy trabajando y cuál es **"mi compromiso adquirido en la Daily"**. Todo lo que no contribuya con esto último debe ser evitado. Nuestro compromiso seguirá un sistema de arrastre (como en [kanban](https://es.wikipedia.org/wiki/Kanban_(desarrollo))).

En general, debemos mantener el `Sprint Backlog` con las tareas superiores asignadas (Work In Progress - WIP) que deberían estar terminadas en la siguiente Daily (porque estos elementos tienen una duración de 1 día o menos) y cuando se completan pasan a la última columna de incidencias cerradas.

Es mejor finalizar una tarea y compartir los cambios con el equipo que estar trabajando en tres tareas al mismo tiempo (es decir, la visualización deseable es tener una tarea asignada que esté en lo más alto de **La Pila**, cualquier otra visualización debe hacernos pensar).

En caso de no poder cerrar un issue directamente con un commit, se puede arrastrar el issue a la columna de cerrados. Así nuestro tablero será la herramienta principal para visualizar y gestionar el estado de las tareas.

> _NOTA: Se pueden crear otras columnas intermedias para otros estados (como por ejemplo pendiente de test de integración si hay dependencias de otras tareas)._
