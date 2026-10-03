# Problem Brief

## Decisión del problema

### Problema elegido

> El problema ganador en una frase, sin mencionar blockchain, y quién lo propuso.

La trazabilidad de las actividades de mantenimiento y reparación de aeronaves depende de registros manuales y documentos firmados físicamente, dificultando verificar quién realizó, inspeccionó y aprobó cada intervención a lo largo del tiempo.

### Por qué elegimos este

> Qué inclinó al equipo por este problema frente a los demás, según los criterios de la Sesión 1.

El equipo consideró que este problema tiene un alto impacto operativo y regulatorio porque afecta auditorías, cumplimiento FAA/EASA, investigaciones de discrepancias y reconstrucción del historial de mantenimiento. Además, involucra múltiples áreas de negocio (Mantenimiento, Calidad, Ingeniería y Operaciones) y presenta oportunidades claras de mejora en eficiencia, trazabilidad y confianza de los registros.

### Propuestas descartadas

> Cada propuesta considerada, quién la propuso y el motivo del descarte.

El equipo ya contaba con un proyecto predefinido y validado antes del inicio del bootcamp. Se priorizó dar continuidad a la idea original, por lo que no se requirió la apertura de debates sobre nuevas alternativas.

### Cómo tomamos la decisión

> Cómo llegó el equipo al acuerdo: votación, consenso tras debate u otro.

La elección del proyecto se basó en una planificación previa al inicio del bootcamp. Al contar con una idea predefinida y alineada con nuestros objetivos, el equipo determinó de mutuo acuerdo dar continuidad a su desarrollo durante el programa.

---

## Problem Brief

### Encabezado

> Nombre del proyecto y una frase que describa el problema. Extensión: breve.

Tracium - Trazabilidad verificable del mantenimiento aeronáutico

### Equipo y roles

> Integrantes con su usuario de GitHub, rol asumido por cada persona, responsable de las entregas y canal de coordinación interna. Extensión: breve.


| Integrante | Usuario de GitHub | Rol asumido | Responsabilidad |
|---|---|---|---|
| Diego Rubio Ramos | `drubio35` | Coordinación del brief y análisis del problema | Consolidar el documento, mantener la coherencia del caso de negocio y coordinar la integración final. |
|Abdul Ruiz Saldaña | `darienabdul`|Dearrollador | Revisión técnica y planificación de proyectos a nivel de infraestructura.|

### Problema y evidencia

> Enunciado del problema en una frase, sin mencionar blockchain. Contexto, frecuencia y alcance. Evidencia mínima de que el problema existe: observación directa, experiencia propia, conversaciones o fuentes consultadas, con enlace o cita cuando aplique. Extensión: 150–300 palabras.

La trazabilidad, auditoría y verificación de las intervenciones de mantenimiento aeronáutico se ven obstaculizadas por la fragmentación de la información crítica entre registros manuales, documentación física firmada y sistemas de información aislados. Este problema se manifiesta de forma crítica cada vez que un operador, auditor o autoridad reguladora necesita validar el historial completo de un componente o aeronave, incluyendo la identidad del técnico ejecutor, el inspector asignado, la aprobación del retorno al servicio (RTS) y el historial de modificaciones posteriores. 

Aunque la frecuencia de estas búsquedas, el tiempo medio de resolución (MTTR) y la cantidad exacta de plataformas desconectadas están pendientes de medición cuantitativa, el impacto operativo en la eficiencia y la gestión del riesgo es inmediato.La evidencia preliminar se sustenta en la observación directa de los flujos de trabajo actuales descritos por el proponente, donde predomina el uso de firmas autógrafas en soportes físicos, sin una certeza operativa de que los metadatos de ejecución, control de calidad y enmiendas se consoliden de manera íntegra en una base de datos unificada.

La criticidad de esta brecha está respaldada por el marco regulatorio internacional; las directrices de la FAA sobre el mantenimiento de registros exigen una atribución inequívoca y la preservación a largo plazo de los datos, mientras que la normativa EASA Parte 145 establece controles estrictos sobre la gestión de registros y la seguridad de los sistemas electrónicos.

Para validar la magnitud del problema, la investigación subsiguiente contempla un enfoque metodológico basado en la observación directa en campo, el análisis de una muestra representativa de paquetes de trabajo (Work Packages), el mapeo de la arquitectura de sistemas actual y la conducción de entrevistas semiestructuradas con los líderes de Mantenimiento, Aseguramiento de la Calidad y Control de Registros

### Usuario y actores

> Quién sufre el problema y qué necesita resolver. Cómo lo resuelve hoy y qué le cuesta en dinero, tiempo o esfuerzo. Demás actores que intervienen en el flujo, con el papel que cumple cada uno. Extensión: 150–300 palabras.

Los usuarios principales son los técnicos de Mantenimiento, que registran intervenciones y evidencias, y los auditores internos o regulatorios, que necesitan reconstruir y validar el historial de una intervención. El problema se manifiesta cuando el técnico debe dejar evidencia completa y vinculada de su trabajo, o cuando el auditor necesita comprobar quién ejecutó, inspeccionó y aprobó una actividad sin navegar entre órdenes de trabajo, tarjetas de tarea, logbooks, formularios firmados, documentos escaneados y datos almacenados en aplicaciones. Como usuarios secundarios participan Calidad, Ingeniería, Operaciones y Cumplimiento Regulatorio. Hoy la respuesta puede requerir localizar documentos, interpretar firmas, confirmar revisiones y reconciliar información que no está vinculada mediante un identificador común. El costo exacto todavía debe medirse, pero incluye tiempo de personal, esperas, reprocesamiento y riesgo de utilizar información incompleta.

Los actores directos son la persona que ejecuta el trabajo, la persona que inspecciona, quien certifica o aprueba el retorno al servicio y quien archiva o administra el paquete. Los actores indirectos incluyen Ingeniería, administradores de aplicaciones, auditoría interna, operadores, clientes y autoridades regulatorias cuando solicitan evidencia. Cada actor cumple una función distinta: producir el dato, verificarlo, aprobarlo, custodiarlo o consultarlo.

La investigación debe evitar asumir que todos padecen la misma fricción. Las entrevistas deberán identificar qué documento consideran oficial, qué información duplican, qué permisos poseen y en qué punto dejan de confiar en el registro disponible.

### Flujo actual de valor

> Recorrido paso a paso de cómo se mueve hoy el dinero, la información o el activo, desde el origen hasta el destino. Diagrama o secuencia numerada, con los intermediarios explícitos. Señalar si algún paso responde a una obligación normativa. Extensión: 150–300 palabras.

1. El operador o el personal autorizado identifica una discrepancia o necesidad de mantenimiento.
2. Se abre una orden de trabajo, squawk, tarjeta o documento equivalente y se identifica la aeronave o el componente.
3. Mantenimiento consulta los datos técnicos aplicables y ejecuta la intervención.
4. La persona que realiza el trabajo documenta la actividad y firma o identifica la finalización según el procedimiento aplicable.
5. Cuando corresponde, otra persona inspecciona el trabajo y registra el resultado.
6. Personal autorizado revisa la documentación y aprueba el retorno al servicio o la certificación correspondiente.
7. El paquete se recopila, revisa y archiva. Parte de la evidencia puede escanearse o registrarse en uno o varios sistemas.
8. Más adelante, Calidad, Ingeniería, Operaciones, el cliente o una autoridad solicita el historial.
9. Una persona busca los registros, conecta documentos y datos, verifica firmas y revisiones, y prepara una respuesta o reporte.

El valor se mueve como confianza documentada: desde la ejecución técnica hasta la capacidad de demostrar qué ocurrió. La información se mueve mediante documentos, firmas, archivos escaneados y posibles registros de aplicaciones. Calidad y las funciones de autorización actúan como intermediarios necesarios. El paso de archivo y reconciliación puede ser un intermediario evitable si la misma evidencia se captura y vincula correctamente desde el origen. Algunos controles, sin embargo, responden a obligaciones normativas o procedimientos aprobados y no deben eliminarse sin validación.

### Fricciones identificadas

> Puntos concretos donde el flujo falla, se encarece o se demora. Cada fricción indica en qué paso ocurre, qué la causa y a quién afecta. Extensión: 150–300 palabras.

La primera fricción es la fragmentación. Un mismo evento puede aparecer en una orden de trabajo, una tarjeta, una entrada de logbook, un archivo escaneado y una aplicación. Si esos elementos no comparten identificadores y revisiones controladas, reconstruir el evento exige búsquedas y comparaciones manuales. La causa potencial es que cada documento cumple una finalidad distinta y el proceso no fue diseñado como una cadena digital de trazabilidad. Afecta principalmente a Calidad, Ingeniería y a quien prepara evidencia para auditoría.

La segunda fricción es la atribución. Una firma manual puede demostrar aprobación en el documento físico, pero resulta más difícil utilizarla para búsquedas, validaciones automáticas o análisis históricos. La causa no es la firma en sí, sino la falta de una relación estructurada entre la identidad, la función, la autorización, la fecha y la versión exacta del registro.

La tercera fricción es el control de cambios. Todavía debe verificarse si los sistemas actuales conservan valores anteriores, autor de la modificación, fecha, motivo y aprobación. Sin esta información, una corrección puede ser difícil de distinguir de una alteración no autorizada.

La cuarta fricción es la incertidumbre sobre la fuente oficial. Si el papel, el archivo escaneado y la base de datos muestran información diferente, el usuario necesita saber cuál prevalece y cómo se resolvió la discrepancia.

### Oportunidad e hipótesis

> Oportunidad priorizada entre las fricciones identificadas, con el motivo de la elección. Hipótesis inicial de por qué blockchain podría mejorar ese punto, expresada en términos de qué cambiaría para el usuario. Extensión: 150–300 palabras.

**Oportunidad priorizada**

La oportunidad priorizada consiste en facilitar la reconstrucción y verificación del historial de mantenimiento aeronáutico mediante una trazabilidad digital que vincule cada intervención con sus evidencias de ejecución, inspección, aprobación y modificaciones posteriores. Esto permitiría reducir el esfuerzo de búsqueda y reconciliación de documentos, así como la incertidumbre sobre la procedencia, integridad y validez de los registros consultados. Se prioriza esta oportunidad porque aborda directamente las fricciones de fragmentación, atribución y control de cambios identificadas en el proceso actual, cuyo impacto deberá cuantificarse durante la investigación.

**Hipótesis inicial**

La hipótesis es que un registro distribuido basado en blockchain, compartido entre organizaciones autorizadas, podría mejorar la verificabilidad del historial de mantenimiento al permitir comprobar la secuencia, integridad y procedencia de los eventos registrados, sin depender exclusivamente de la custodia de una única organización. Para el usuario, esto se traduciría en pasar de localizar y reconciliar evidencias dispersas a consultar un historial vinculado y verificable, reduciendo el tiempo de búsqueda y facilitando la identificación de modificaciones posteriores.

Esta hipótesis depende de confirmar que varias organizaciones independientes necesitan validar un mismo historial y que no existe un custodio central aceptado por todas. Además, deberá evaluarse frente a alternativas como una base de datos centralizada con firmas electrónicas, control de acceso, versionado e integración entre sistemas. La validación medirá el tiempo de reconstrucción del historial, la integridad verificable de los registros y la capacidad de identificar modificaciones no autorizadas. Blockchain solo se justificará si demuestra ventajas concretas frente a estas alternativas.

### Criterio de pertinencia

> Justificación de por qué el caso requiere un registro distribuido y no una base de datos tradicional o una integración entre sistemas existentes. Debe apoyarse en al menos uno de los criterios de la Sesión 1: varias partes que no confían entre sí necesitan compartir un mismo registro, el histórico no puede alterarse, o se elimina un intermediario que hoy concentra la confianza. Extensión: 150–300 palabras.

La pertinencia de un registro distribuido dependerá de confirmar que varias organizaciones independientes, como operadores, organizaciones de mantenimiento y centros de servicio, necesitan compartir y validar el historial de mantenimiento de una aeronave o componente, sin que exista un custodio central aceptado por todas. En este escenario, cada participante requiere confiar en la integridad y procedencia de los registros, así como verificar que las intervenciones, inspecciones, aprobaciones y correcciones posteriores correspondan con la secuencia de eventos registrada.

Un registro distribuido basado en blockchain podría aportar valor al permitir que los participantes autorizados verifiquen la integridad y el orden de los eventos sin depender exclusivamente de la base de datos o de la custodia de una sola organización. La conservación de los registros anteriores y la trazabilidad de las modificaciones permitirían identificar cambios posteriores y mantener evidencia verificable del historial. Esto no sustituye los controles de calidad, las autorizaciones del personal ni las obligaciones regulatorias aplicables, y tampoco garantiza que la información registrada sea correcta desde su origen.

La pertinencia tecnológica deberá validarse frente a una alternativa centralizada que incorpore firmas electrónicas, control de acceso, versionado, auditoría e integración entre sistemas. Si una organización es aceptada por todos como custodio, o si las soluciones existentes permiten compartir y verificar el historial con suficiente confianza, un registro distribuido podría añadir complejidad sin un beneficio proporcional.

Por tanto, el proyecto avanzará con blockchain únicamente si la investigación demuestra necesidades de confianza compartida entre organizaciones, verificabilidad del historial y ventajas concretas frente a las alternativas centralizadas.

### Supuestos y riesgos

> Dos o tres supuestos que tendrían que ser ciertos para que la hipótesis funcione, y qué podría invalidarla. Extensión: 150–300 palabras.

**Supuesto 1:** la información crítica está fragmentada y no existe ya un historial digital completo. Este supuesto podría invalidarse si la base de datos actual conserva ejecución, inspección, aprobación, versiones y cambios con suficiente trazabilidad. En ese caso, el problema real sería acceso, integración, capacitación o uso del sistema, no ausencia de trazabilidad.

**Supuesto 2:** varias organizaciones independientes necesitan validar el mismo registro y no aceptan plenamente a un custodio central. Podría invalidarse si el proceso ocurre dentro de una sola organización o si los clientes y autoridades aceptan el sistema actual como fuente oficial. En ese escenario, una arquitectura centralizada probablemente sería más simple.

**Supuesto 3:** el costo de búsqueda, reconciliación y preparación de evidencia es material. Podría invalidarse si las consultas son poco frecuentes, rápidas o ya están automatizadas. Deben medirse tiempo de búsqueda, número de transferencias, documentos consultados y casos de información inconsistente.

Los riesgos incluyen almacenar datos sensibles o personales en un registro difícil de corregir; confundir inmutabilidad con exactitud, ya que un dato incorrecto puede registrarse de forma permanente; duplicar sistemas existentes; crear dependencia de integraciones; y diseñar una solución que no sea aceptada por Calidad o por los procedimientos aprobados. Otro riesgo es usar blockchain como objetivo y no como hipótesis. La mitigación inicial es mapear el proceso, clasificar los registros, confirmar la fuente oficial y comparar alternativas antes de seleccionar arquitectura.
