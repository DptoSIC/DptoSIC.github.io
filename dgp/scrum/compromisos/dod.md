# Definición de Hecho (`Definition of Done - DoD`)

La **`DoD`** es una **descripción formal del estado del** `Incremento` **cuando cumple con las medidas de calidad requeridas para el producto**.

En el momento en que un elemento de trabajo pendiente de producto (`PBI`) cumple con la **`DoD`**, se crea un `incremento`.

La **`DoD`** crea transparencia al proporcionar a todos una comprensión compartida de qué trabajo se completó como parte del `Incremento`. Si un `PBI` no cumple con la **`DoD`**, no se puede liberar, ni siquiera presentar en la <span style="text-decoration: underline">Sprint Review</span>. En su lugar, vuelve al `Product Backlog` para su consideración futura.

Si la **`DoD`** para un `incremento` forma parte de los estándares de la organización, todos los equipos de Scrum deben seguirla como mínimo. Si no es un estándar organizativo, el equipo de Scrum
debe crear una **`DoD`** adecuada para el producto.

Los desarrolladores deben ajustarse a la **`DoD`**. Si hay varios equipos de Scrum trabajando juntos en un producto, deben definir y cumplir mutuamente con la misma **`DoD`**.

## Cuidado con la deuda técnica

Cuando se dan por finalizados elementos que no cumplen con la **`DoD`** se empieza a acumular deuda técnica. Cumplir la **`DoD`** no garantiza no tener deuda técnica. Si aún cumpliendo la **`DoD`** se acumula deuda técnica puede ser un indicador de que la **`DoD`** no es correcta y hay que revisarla.

**La deuda técnica reduce la capacidad de generar valor** según el siguiente gráfico.

![Lucha con la deuda técnica](/imgs/lucha-con-deuda-tecnica.webp)

Algunos puntos que debería tener la **`DoD`** son:
1. Test (aceptación, [regresión](https://es.wikipedia.org/wiki/Pruebas_de_regresi%C3%B3n), integracion, rendimiento, estabilidad, etc...). Deberían automatizarse.
1. Refactoring
1. Release notes
1. Documentación de usuario
1. Localizaciones para audiencias objetivo
1. Code reviews

## Lecturas recomendadas

![Lecturas DoD](/imgs/lecturas-dod.webp){:.centered}