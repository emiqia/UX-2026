# Retroalimentación de evaluaciones que el estudiante efectivamente utilice

Repositorio de documentación del proyecto UX del **grupo 5**. El proyecto busca que la retroalimentación de una evaluación se convierta en una corrección concreta en la siguiente entrega y permita comprobar la evolución del estudiante por criterio de rúbrica.

## Integrantes

| Integrante |
| --- |
| Cristian Sandova |
| Emilia Toro |
| Bastian Wenckhans |

## Proyecto seleccionado

La retroalimentación de trabajos y rúbricas llega tarde y dispersa entre comentarios en PDF, planillas y correos. Esto dificulta que el estudiante comprenda qué falló y aplique los comentarios antes de su siguiente entrega.

El desafío consiste en **cerrar el ciclo de retroalimentación**: identificar el criterio que falló, entender qué acción concreta lo corrige y comprobar si hubo una mejora respecto de la entrega anterior. La superficie funcional es pequeña; el foco del diseño está en la claridad de la información y en la evidencia de uso de la retroalimentación.

### Historia de usuario principal

> Como estudiante que obtuvo una nota baja en la primera entrega, necesito ver exactamente qué criterio falló y qué debo hacer distinto en la próxima, para no repetir el mismo error sin darme cuenta.

### Objetivo de diseño

Diseñar una experiencia que conecte **criterio evaluado → dificultad detectada → acción de mejora → evidencia de aplicación → resultado de la siguiente entrega**.

La propuesta de valor es ayudar al estudiante a transformar los comentarios de una evaluación en acciones comprensibles y verificables para su siguiente trabajo.

El [contexto del proyecto](docs/project-brief.md) desarrolla el problema, el alcance propuesto y las preguntas que deberán validarse con usuarios.

## Actividades realizadas

### 1. UX personas

Se elaboraron **tres perfiles distintos**, con áreas, instituciones y roles diferentes. Dos representan a los estudiantes que reciben y aplican la retroalimentación; el tercero representa a la docente que la entrega y revisa la evidencia de corrección.

Son **personas preliminares o proto-personas**. Las características e instituciones forman parte del escenario de diseño y deben validarse con usuarios; no representan participantes entrevistados ni una implementación institucional. Los materiales compartidos no incluyen registros de entrevistas, encuestas o pruebas.

| Persona | Edad | Área y rol | Institución | Relación con la solución |
| --- | --- | --- | --- | --- |
| Valentina Rojas | 20 | Estudiante de ingeniería informática; usuaria principal. | Universidad de La Frontera | Identifica el criterio que falló, sigue una acción correctiva y compara su resultado en la siguiente entrega. |
| Samon Baker | 21 | Estudiante de diseño gráfico y practicante; usuario principal. | INACAP | Reúne comentarios por proyecto, prioriza revisiones y vincula cada acción con evidencia del cambio en su diseño. |
| Martina Soto | 29 | Docente universitaria del área de educación; usuaria secundaria. | Universidad Católica de Temuco | Relaciona comentarios con criterios y acciones, revisa la evidencia de corrección y compara resultados entre entregas. |

Los tres perfiles se sitúan en Temuco, Chile. Sus diferencias orientan necesidades de interacción concretas: claridad para Valentina, priorización para Samon y seguimiento de la aplicación para Martina.

#### Valentina Rojas

![Valentina Rojas, estudiante de ingeniería informática de la Universidad de La Frontera: comprensión y aplicación de la retroalimentación](ux-personas/1.png)

#### Samon Baker

![Samon Baker, estudiante de diseño gráfico de INACAP y practicante: priorización de revisiones y evidencia de cambios](ux-personas/2.png)

#### Martina Soto

![Martina Soto, docente de la Universidad Católica de Temuco: acciones correctivas y verificación del progreso](ux-personas/3.png)

[Consultar el PDF de las tres UX personas](docs/user-personas.pdf).

Las fichas están en inglés y comparten una estructura de información personal, biografía, objetivos, frustraciones, personalidad, intereses y necesidades. La composición utiliza fotografía a la izquierda e información en dos columnas a la derecha. Sobre las fotografías se muestra únicamente el nombre; el área, la institución y el rol aparecen en la información personal.

### 2. Value Proposition Canvas

El canvas relaciona las tareas, frustraciones y beneficios esperados del estudiante con funcionalidades y mecanismos propuestos para facilitar el uso de la retroalimentación.

![Value Proposition Canvas del proyecto de retroalimentación de evaluaciones](value_proposition.png)

[Consultar el PDF original del canvas](docs/value-proposition-canvas.pdf).

| Componente | Contenido del canvas actual |
| --- | --- |
| Tareas del estudiante | Organizar su agenda académica, conocer los criterios de evaluación, comprender errores previos y ejecutar acciones correctivas en entregas posteriores. |
| Frustraciones | Información fragmentada, desconocimiento de parámetros de evaluación, retroalimentación tardía y comentarios ambiguos. |
| Beneficios esperados | Claridad sobre los pasos de mejora, evidencia de progreso, centralización de información y transparencia de la evaluación. |
| Productos y servicios | Panel académico, módulo de rúbricas, panel de progreso y vinculación de criterios fallidos con acciones correctivas. |
| Aliviadores de frustraciones | Transformar comentarios abstractos en orientaciones accionables, mostrar la rúbrica anticipadamente y reunir información académica. |
| Creadores de beneficios | Facilitar la autoevaluación, orientar el tiempo de estudio y mostrar la evolución del estudiante. |

El vínculo entre criterio y acción correctiva responde directamente al problema. Para la siguiente iteración se propone priorizarlo junto con la evidencia de aplicación y la comparación por criterio. La agenda, los horarios y la centralización de toda la información académica son funciones complementarias que requieren justificar su aporte al objetivo principal.

## Alcance funcional propuesto

Estas funciones describen la dirección de diseño para un prototipo; su implementación y validación están pendientes.

1. **Revisión de la evaluación:** consultar criterios, nivel o puntaje obtenido y comentario asociado.
2. **Acción de mejora:** entender qué cambiar, por qué y cómo reconocer que la corrección está realizada.
3. **Registro de aplicación:** vincular la acción con un fragmento, sección o cambio concreto de la siguiente entrega.
4. **Comparación entre entregas:** revisar el resultado del mismo criterio cuando las rúbricas sean comparables.

La experiencia inicial puede concentrarse en una asignatura y dos entregas relacionadas. La docente actúa como usuaria secundaria: vincula comentarios a criterios y acciones, y revisa la evidencia aportada por el estudiante. Las notificaciones pueden ayudar a conocer la disponibilidad de comentarios, pero no demuestran que estos se comprendieron o se aplicaron.

## Recorrido principal propuesto

1. El estudiante abre la retroalimentación de su primera entrega.
2. Identifica un criterio que no alcanzó el nivel esperado.
3. Revisa una explicación y una acción concreta de mejora vinculadas a ese criterio.
4. Aplica la acción en la siguiente entrega y registra dónde realizó el cambio.
5. La docente revisa el cambio vinculado a la acción y evalúa la nueva entrega.
6. El estudiante compara el resultado de ese criterio con el de la entrega anterior, cuando las rúbricas son equivalentes.

### Ejemplo ilustrativo

Este ejemplo sirve para explicar la propuesta; no corresponde a un hallazgo ni a una prueba realizada.

| Paso | Ejemplo |
| --- | --- |
| Criterio | Justificación de decisiones de diseño. |
| Dificultad | La primera entrega presenta una decisión sin vincularla a evidencia de usuarios. |
| Acción concreta | Añadir la evidencia que respalda la decisión y explicar su relación con el problema del usuario. |
| Evidencia de aplicación | Señalar la sección de la segunda entrega donde se incorporó esa justificación. |
| Comprobación | Revisar el nivel alcanzado en el mismo criterio en la segunda evaluación. |

## Trazabilidad de las decisiones de diseño

La siguiente tabla vincula necesidades descritas en los materiales con propuestas de diseño y formas de validarlas. No representa resultados de investigación.

| Necesidad o dificultad | Respuesta propuesta | Evidencia a recoger |
| --- | --- | --- |
| No saber qué criterio falló | Presentar criterio, resultado y comentario juntos. | El estudiante identifica correctamente el criterio y explica la dificultad. |
| No entender qué corregir | Mostrar una acción específica y un ejemplo pertinente. | El estudiante explica con sus palabras qué cambiará. |
| Revisar archivos y correos separados | Reunir la retroalimentación de la entrega en una vista. | Localiza el comentario relevante sin recorrer varias fuentes. |
| Repetir errores | Vincular acciones de mejora con evidencia en la siguiente entrega. | Se identifica un cambio concreto asociado al comentario anterior. |
| No reconocer el progreso | Comparar el resultado del mismo criterio entre entregas. | Reconoce si el desempeño mejoró, se mantuvo o empeoró. |
| Poco tiempo para revisar proyectos de diseño | Priorizar acciones y reunir comentarios por versión. | El estudiante encuentra una acción relevante y señala el cambio realizado. |
| Dificultad docente para comprobar la aplicación | Vincular evidencia de la siguiente entrega con cada comentario anterior. | La docente identifica la corrección y la evalúa respecto del mismo criterio. |

## Validación propuesta

Se propone evaluar el prototipo con estudiantes de ingeniería y diseño que hayan recibido retroalimentación y deban realizar una entrega posterior relacionada. La participación de docentes permitirá revisar la claridad de las acciones y el esfuerzo de verificar las correcciones. Una prueba inicial puede pedirles localizar un criterio débil, explicar la corrección, registrar evidencia y leer la comparación entre entregas.

| Dimensión | Indicador propuesto |
| --- | --- |
| Comprensión del problema | Proporción de participantes que identifica correctamente el criterio que debe mejorar. |
| Claridad de la acción | Proporción que describe una corrección concreta coherente con el comentario y la rúbrica. |
| Facilidad de uso | Tiempo, errores y ayuda requerida para encontrar y comprender la retroalimentación. |
| Aplicación | Proporción de acciones que cuenta con evidencia pertinente en la siguiente entrega. |
| Evolución | Cambio de nivel o puntaje del mismo criterio entre evaluaciones comparables. |

**Abrir un comentario o marcar una tarea como realizada no demuestra por sí solo que se aplicó la retroalimentación.** Esa aplicación requiere evidencia en el trabajo. Una mejora de nota tampoco demuestra, por sí sola, que la herramienta causó la mejora. Las metas numéricas y el tamaño de las pruebas se definirán al preparar la investigación.

## Estado y próximos pasos

| Actividad | Estado |
| --- | --- |
| Definición inicial del problema y de la historia de usuario | Disponible. |
| Elaboración de UX personas | Tres perfiles actualizados en inglés, con roles e instituciones distintos; validación pendiente. |
| Elaboración del Value Proposition Canvas | Disponible; requiere priorización del alcance. |
| Investigación con estudiantes y docentes | Pendiente; no se adjuntó evidencia. |
| Diseño de flujos y prototipos | Propuesto; no se adjuntaron prototipos. |
| Pruebas de usabilidad y seguimiento de aplicación | Pendiente. |
| Propuesta de interfaz de alta fidelidad | Pendiente. |

Los siguientes pasos son validar las necesidades de los tres perfiles con estudiantes y docentes, ajustar el canvas al ciclo de retroalimentación y diseñar un prototipo que permita comprobar la relación entre comentario, corrección y entrega posterior.

## Contenido del repositorio

```text
.
├── README.md
├── docs/
│   ├── project-brief.md
│   ├── user-personas.pdf
│   └── value-proposition-canvas.pdf
├── ux-personas/
│   ├── 1.png
│   ├── 2.png
│   └── 3.png
└── value_proposition.png
```

La documentación principal está en español. Las tres fichas de personas y su PDF están en inglés. El canvas conserva el contenido y el idioma del archivo entregado; su siguiente iteración deberá considerar los tres perfiles actuales.

Este repositorio documenta una propuesta UX. Los archivos entregados no incluyen una aplicación ejecutable, por lo que no hay instrucciones de instalación ni ejecución.
