# Estudio de Viabilidad del Sistema (EVS)

El [Estudio de Viabilidad del Sistema (EVS)](https://es.wikipedia.org/wiki/An%C3%A1lisis_de_viabilidad) básicamente trata de qué se puede hacer en la situación actual.

Partiendo de la información disponible se obtendrán los siguientes puntos clave:
1. Los [**requisitos** detectados](https://dim.institutomilitar.com/shared/NIeUthgV0xdIKPlkK9CXDGS1bjnbN1aoU8O1nqVb18D),
1. los [**riesgos**](https://es.wikipedia.org/wiki/Riesgo) valorados (tanto en probabilidad de materializarse como daño sobre el sistema) y su aplicación en cada caso (puede que sea un riesgo sólo para una alternativa como desplegar en una Intranet),
1. las **preguntas** que queden pendientes para aclarar (ver abajo) con los todos los stackeholders y
1. delimitar el objetivo inicial del estudio que debe responder a **¿Cuál es el MVP?**

> Otros conceptos relacionados son:
> 1. [Time to Market (TTM)](https://en.wikipedia.org/wiki/Time_to_market)
> 1. [Retorno de la Inversión (ROI)](https://en.wikipedia.org/wiki/Return_on_investment)

> _NOTA DIM: Es recomendable **hacer ya en este punto un borrador de Diagrama de Casos de Uso (CU) y de Modelo de Dominio**. No deben estar demasiado detallados ya que no son documentos de trabajo para implementación (puede que la alternativa escogida sea comprar una aplicación, pero sirven para analizar mejor alternativas de terceros y comprender bien el alcance del negocio y las relaciones entre actores, procesos y entidades. **Sobretodo son muy útiles inicialmente en nuestro caso ya que se ha observado en muchos alumnos que comprenden mejor sus proyectos individuales si pueden visualizar esta información**._

Las reuniones con los stackeholders hay que preparalas muy bien si no se dispone de ellos a diario. Estos son algunos consejos importantes:
1. **Opciones** sobre las que tenga que decidir: _"Esto se puede hacer así o así"_ y **el cliente debe decidir**.
1. **Implicaciones / Acciones derivadas**, sobretodo en las preguntas que añadan esfuerzo adicional: _"Si quiere que también tenga esta funcionalidad implicará X coste adicional y/o retrasar X tiempo la entrega y/o tener autorización de X, etc..."_. **De lo contrario el cliente siempre dirá que sí a un producto mayor** si no conoce el coste.
1. **Todo debe estar anotado** previamente, no sólo por tener una guía a la hora de desarrollarse la reunión y tener una estructura coherente que no haga saltar de un tema a otro y volver, sino porque puede que la reunión no sea con todo el equipo y nuestro representante debe tener perfectamente claro el objetivo de la pregunta que se debe responder y la información que debe tener el cliente para tomar la decisión. Es deseable levantar un acta de la reunión y apuntar los asistentes ya que durante el desarrollo podrían cambiar los stackholders. En algunos órganos de desarrollo el acta se firma y pasa a formar parte de la documentación del proyecto. Este punto no debe entenderse como un contrato o para añadir rigidez frente a los cambios sino **para conseguir transparencia y trazabilidad**.
1. **Definir bien los términos usados**. Por ejemplo, un evento deportivo tratado como histórico ¿Es un dato conseguido de una web donde se vuelca con X frecuencia o es cualquier partido finalizado? Dependiendo cómo se entienda hay o no diferencia con tratarlo como un dato en vivo.
1. Para trabajar con el cliente **también es útil la herramienta [Customer Journey](https://en.wikipedia.org/wiki/Customer_experience#Customer_journey_mapping)** (traducido como [mapa de experiencia del cliente](https://www.syndesis.mx/post/2017/01/08/mapa-de-la-experiencia-del-cliente)). Se aprovecha más si estamos muy enfocados desde el principio, ya que puede ampliar información que nos haya llegado sesgada y puede originar soluciones que no se habían tenido inicialmente en cuenta. Aunque como desarrolladores no es trabajo nuestro abarcar todas las etapas del viaje, sí que nos va a ayudar a conocer cuál será el usuario que usará la aplicación y qué experiencia debemos mejorar con respecto a la situación actual, priorizando las funcionalidades que tengan más impacto o nos aporten más información de cara a definir el MVP (ver [video de ejemplo](https://www.youtube.com/watch?v=PTk_KncCivE)).  
![Esquema Customer Journey map](https://uxpressia.com/examples/export/cjm/cjm.png)
1. **Evitar ampliar el alcance** dando nuevas ideas ya que se trata de reducir la incertidumbre y definir el MVP. Si el desarrollo es de calidad será fácilmente adaptable a lo que requiera el mercado. Es mejor una buena solución hoy que la mejor más tarde (normalmente demasiado tarde). La oportunidad es una virtud muy valiosa.

## Alternativas de solución
Se deben elaborar las alternativas que proporcionan una solución. Cada una con los siguientes puntos:
1. Definición de **arquitectura y tecnología** (de cada entorno en su caso)
1. **Estimación** de carga de trabajo y plazos de tiempo asociados.
1. **Valoración económica** (mano de obra, hardware, software y servicios externos). Evidentemente debe ser coherente con la estimación.
1. **Riesgos** valorados para la alternativa concreta. Debe haber una propuesta de evitarlo, minimizarlo o reponerse ante su impacto.
1. **Licenciamiento** de los distintos subsistemas que forman el producto. [Puede venir impuesto](https://en.wikipedia.org/wiki/Comparison_of_free_and_open-source_software_licences) por las dependencias de cada solución. Si no es compatible debe añadirse el coste de la alternativa a cada subsistema en conflicto.
1. Cualquier otro aspecto específico con gran impacto en el desarrollo.

**Al final del EVS hay una reunión con el cliente donde se le plantean las alternativas** de solución acompañadas de una matriz de decisión ponderada sobre los aspectos relevantes desde el punto de vista del cliente (igual que la que se hace en el método de planeamiento táctico) **y debe elegir una o dirigir un nuevo estudio en otra dirección** si ninguna solución le parece adecuada.

Hay muchos ejemplos de EVS en los [proyectos finales](https://git.institutomilitar.com/proyectos-finales) de otros años, aunque lo mejor no es coger una plantilla sino recoger lo que le puede interesar al cliente y pueda entendernos de la forma más rápida.

> _NOTA: El formato para definir un requisito es:_  

| ID | Descripción | Prioridad | Fuente |
|---|:---|---|:---|
| Nº | Definición que deje claro la "DoD" | Se puede omitir si están ordenados | Enlace a documento o dónde defina qué persona lo ha incluido |
| 1 | Importar datos de football-data | Alta | [Doc 1](https://16khs695mehu6grk1ykq.institutomilitar.com/Requisitos%20Datos%20Deportivos.docx) |
| 2 | Basado en tecnología serverless para ahorrar costes iniciales | Media | [Doc 2](https://github.com/DptoSIC/DatosDeportivos) |  

