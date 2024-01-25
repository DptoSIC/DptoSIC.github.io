
# Especificación de Requisitos de Software (ERS)

Una vez que se ha tomado la decisión, sobre qué solución interesa más, se hace la [Especificación de Requisitos de Software (ERS)](https://es.wikipedia.org/wiki/Especificaci%C3%B3n_de_requisitos_de_software).

Normalmente los requisitos ya se han trabajado de manera general en el EVS y en esta parte se refinan, ajustan o descartan conforme a la solución escogida.

## Formato

El formato para definir un requisito habitualmente en el MINISDEF es el de la siguiente tabla:  

| ID | Descripción | Prioridad | Fuente |
|---|:---|:---|:---|
| Nº | Debe dejar claro el valor que aporta | Se puede omitir si están ordenados | Enlace a documento o dónde defina qué persona lo ha incluido |
| 1 | Importar datos de football-data | Alta | [Doc 1](https://16khs695mehu6grk1ykq.institutomilitar.com/Requisitos%20Datos%20Deportivos.docx) |
| 2 | Basado en tecnología serverless para ahorrar costes iniciales | Media | [Doc 2](https://github.com/DptoSIC/DatosDeportivos) |  
| 3 | Tamaño mínimo de letra 20px para accesibilidad | Media | STte. Carpanta |  

Este listado es mejor tenerlo en un documento aparte porque afectará a varios documentos y así se puede referenciar y tener una copia única actualizada.

Un listado como este será necesario en la descripción funcional cuando haya que solicitar autorización para un desarrollo (Anexo II de la IT 01/2020 de CESTIC, actualización de 2021), aunque normalmente es un listado que aporta poco a la hora de desarrollar y suele quedar obsoleto una vez se haya implementado parte del producto.

## Herramientas para la extracción de requisitos

Los artefactos con los que vamos a trabajar son:
1. El **Impact Map** y el **Mind Map** son fundamentales para trabajar con el cliente clarificando aspectos importantes que son difíciles de ver en texto y se ven mejor con herramientas visuales. A la hora de adaptar el trabajo pendiente son muy útiles.  
1. El **Diseño de la Interfaz de Usuario** (interfaces comunes - inicialmente dirigidas al MVP). Es un **documento importantísimo y con el que el cliente nos va a dar mayor feedback**. Para crearlos se pueden usar técnicas de Design Thinking como el wireframe.  
![Ejemplo wireframe](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fi.pinimg.com%2Foriginals%2F62%2Fd2%2Fdb%2F62d2db2ced4c7f3923419783c496ba21.jpg&f=1&nofb=1)  
Para ello se pueden usar [herramientas de mockeo](https://blogs.systweak.com/best-mockup-software-and-wireframe-tools/) o simplemente papel y boli. Para tomar decisiones mejor informadas se pueden usar técnicas como los [test A/B](https://es.wikipedia.org/wiki/Prueba_A/B). Es **imprescindible que permita la funcionalidad prevista para el MVP** (de nada sirve tener muchas pantallas si al menos una no hace lo que se ha pedido).  
1. El diagrama de **Casos de Uso (CU)** y el **Modelo de Dominio** nos pueden servir si estamos cómodos con ellos, pero es un documento interno con poco aprovechamiento a la hora de trabajar con el cliente. Durante el curso se piden pues son diagramas que se deben conocer junto con el resto de diagramas de UML, ya sea por proyectos heredados que los tengan en su documentación o porque tengamos que usarlos como parte de supervisión técnica en colaboraciones externas.  
1. Definición y establecimiento de **entornos** (pruebas y producción - _ver punto preproducción_) en su caso.  
1. Solicitud/contrato de servicios externos necesarios para los distintos entornos. La finalidad de empezar con esto es ganar tiempo empezando cuanto antes. En MINISDEF ahora mismo se necesita hacer solicitud del **Anexo II de la IT 01/2020 de CESTIC** (actualización de 2021).

## Requisitos vs La Pila

Con ello se elabora la lista de requisitos para la alternativa escogida (ya que no todas pueden tener los mismos y además sabemos que es un producto vivo). El resultado será nuestro "primer" [Product Backlog o **La Pila**](https://www.scrum.org/resources/what-is-a-product-backlog) (se hablará de ella en Scrum). Cada elemento de **La Pila** que contribuye al MVP debe tener los siguientes elementos (para el resto no hace falta profundizar):
1. Descripción: Suele estar descrita en forma de [Historia de Usuario](https://es.wikipedia.org/wiki/Historias_de_usuario). Lo importante es que quede claro.
1. Valor que aporta: el resto del equipo debe saber que al completar este elemento se tiene acceso a un valor concreto (ejemplo: una funcionalidad nueva)
1. Criterios de aceptación: **La mejor forma de dejarlo claro es definiendo el test que debe superar**. El test se debería realizarse de forma automática en cada commit, no sólo para cerrar el elemento (podría fallar por el nuevo código introducido).
1. Relación con otros elementos:
   1. Riesgos: los riesgos que impacten en el elemento deben quedar claros ya que pueden afectar a su [DoD](https://www.scrum.org/resources/blog/done-understanding-definition-done) (Definición de Hecho, se hablará de ella en Scrum)
   1. Dependencias: cualquier dependencia con otros elementos debe estar satisfecha, ya sea porque esté terminado o se cuente con un [mock](https://es.wikipedia.org/wiki/Objeto_simulado) que satisfaga la dependencia. Puede que estos elementos cambien entre entornos (mock en desarrollo, servicio en producción).
1. Estimación de esfuerzo: En equipos maduros pueden utilizarse distintas técnicas de estimación como los [Puntos de Historia](https://mamaqueesscrum.com/2019/02/25/puntos-de-historia-una-buena-practica-y-una-mala-metrica/) para facilitar las previsiones del equipo, pero lo más útil en el curso es estimar el tiempo que llevará. Se verá cómo refinar elementos hasta que no superen el día. De esa forma en cada [Daily](https://www.scrum.org/resources/what-is-a-daily-scrum) (se hablará de ello en Scrum) se puede actualizar mejor del progreso.

Hay que tener en cuenta que **La Pila** es un documento prioritario y vivo, que debe ser actualizado completamente siguiendo un ciclo como el de la siguiente imagen:  
![Ciclo de evolución de **La Pila**](https://external-content.duckduckgo.com/iu/?u=http%3A%2F%2Fwww.romanpichler.com%2Fwp-content%2Fuploads%2F2012%2F01%2FTheProductBacklogAsALearningTool.jpg&f=1&nofb=1)

Como se ve en la figura, cada retroalimentación conseguida para cada incremento hace evolucionar **La Pila**, por tanto hay que centrarse en los elementos del MVP que es la cantidad mínima de trabajo que nos hará saber si la propuesta es aceptada por "el mercado" o no.