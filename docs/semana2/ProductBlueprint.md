# Product Blueprint

**Nombre del proyecto:** Tracium - Trazabilidad de registros de mantenimiento aeronáutico

**Repositorio (enlace obligatorio):** [tracium_blockchain](https://github.com/darienabdul/tracium_blockchain)

> Los campos marcados como _enlace obligatorio_ deben ir como enlace en Markdown, con este formato: `[texto del enlace](https://...)`. Reemplacen el texto y la dirección de ejemplo.

---

## Contenido

1. Priorización de historias
2. Propuesta de valor
3. Flujo de usuario
4. Alcance del MVP
5. Lean Canvas
6. Backlog priorizado (Kanban)
7. Arquitectura inicial
8. Uso de Stellar y justificación

---

## 1. Priorización de historias

> Historias elegidas entre las que propuso el equipo y criterio con que se priorizaron. Son las que pasan al backlog. Extensión: breve.

## 1. Priorización de historias

> Historias elegidas entre las que propuso el equipo y criterio con que se priorizaron. Son las que pasan al backlog. Extensión: breve.

**Criterio de priorización:** Escriban aquí el criterio (por ejemplo, imprescindible / debería / podría / queda fuera).

Se priorizaron las historias que permiten registrar una intervención desde el origen, consultar su historial completo, comprobar la atribución de las actividades, respaldar el trabajo con evidencia y validar la integridad de los registros:

| Prioridad | Historia                                                                                                                                                                                                                              |        Propuesta por        | Por qué entra al backlog                                                                                                                                                                              |
| :-------: | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :-------------------------: | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|     1     | Como técnico de mantenimiento, quiero registrar una intervención realizada para que quede asociada a mi identidad, fecha y trabajo ejecutado.                                                                                         |     Abdul Ruiz Saldaña      | Es imprescindible porque crea el registro base del producto. Sin la intervención, su autoría y su fecha, no puede existir un historial trazable ni verificable.                                       |
|     2     | Como personal de Calidad, quiero consultar en un solo lugar el historial completo de una intervención de mantenimiento para verificar quién realizó, inspeccionó y aprobó el trabajo.                                                 | Diego Alejandro Rubio Ramos | Es imprescindible porque representa el resultado principal de la solución: reconstruir y verificar el historial sin reconciliar documentos o sistemas dispersos.                                      |
|     3     | Como auditor, quiero verificar quién realizó cada intervención y cuándo fue registrada para poder comprobar la atribución de las actividades.                                                                                         |     Abdul Ruiz Saldaña      | Es imprescindible para establecer responsabilidad y demostrar la procedencia de cada actividad durante una revisión interna o regulatoria.                                                            |
|     4     | Como inspector autorizado, quiero revisar la evidencia del trabajo y registrar el resultado de mi inspección para confirmar que la intervención cumple con los procedimientos aplicables.                                             | Diego Alejandro Rubio Ramos | Debería entrar porque incorpora la validación formal del trabajo y conecta la intervención con la inspección requerida antes de su aprobación.                                                        |
|     5     | Como auditor, quiero verificar la integridad y secuencia de los registros para poder identificar modificaciones posteriores o inconsistencias en el historial.                                                                        |     Abdul Ruiz Saldaña      | Debería entrar porque permite detectar cambios posteriores y comprobar que el historial mantiene una secuencia confiable.                                                                             |
|     6     | Como personal autorizado para el retorno al servicio, quiero verificar que la ejecución y las inspecciones requeridas estén completas antes de registrar mi aprobación para evitar liberar una aeronave con documentación incompleta. | Diego Alejandro Rubio Ramos | Debería entrar porque completa la cadena de responsabilidad y permite confirmar que el trabajo, la evidencia y las inspecciones requeridas estén disponibles antes de aprobar el retorno al servicio. |

---

## 2. Propuesta de valor

> Qué resultado obtiene el usuario y por qué elegiría esta solución. En qué se diferencia de cómo resuelve hoy. Conecta con el usuario del Problem Brief. Extensión: 150–300 palabras en total.

**Usuario (del Problem Brief):**
El usuario principal es el personal de Calidad que necesita reconstruir o validar el historial de una intervención de mantenimiento aeronáutico. También se benefician los técnicos de Mantenimiento, inspectores autorizados, personal de Ingeniería, Operaciones, auditores y personal de Cumplimiento Regulatorio que producen, revisan, aprueban o consultan los registros.

 
**Resultado que obtiene:**
El usuario obtiene un historial digital vinculado y verificable de cada intervención. Desde un mismo punto puede consultar quién realizó el trabajo, cuándo se ejecutó, qué evidencia fue adjuntada, quién inspeccionó la actividad, quién aprobó el retorno al servicio y qué modificaciones se realizaron posteriormente. Esto reduce el esfuerzo necesario para reconstruir el historial y facilita la identificación de información incompleta o inconsistente.

 
**Por qué elegiría esta solución:**
La elegiría porque mejora la trazabilidad, atribución e integridad de los registros sin eliminar los controles de calidad ni las autorizaciones requeridas. Además, facilita la preparación de evidencia para auditorías, investigaciones de discrepancias y revisiones regulatorias. La solución permite validar la procedencia y secuencia de los eventos, manteniendo visibles las correcciones vinculadas al registro original.

 
**En qué se diferencia de cómo lo resuelve hoy:**
Actualmente, el usuario debe buscar y reconciliar manualmente órdenes de trabajo, tarjetas de tarea, logbooks, formularios firmados, documentos escaneados y datos almacenados en diferentes aplicaciones. La solución propuesta captura y relaciona la evidencia desde el origen mediante identificadores comunes, convirtiendo documentos dispersos en un historial estructurado y verificable, sin asumir que la tecnología por sí sola garantiza que los datos registrados sean correctos.

---

## 3. Flujo de usuario

> Recorrido de la persona por la solución de principio a fin, roles y puntos de interacción. Diagrama o secuencia numerada. Extensión: 150–300 palabras.

| Paso | Rol | Qué hace                    | Punto de interacción           |
| :--: | :-: | --------------------------- | ------------------------------ |
|  1   | Rol | Escriban aquí su respuesta. | Pantalla, billetera, red, etc. |
|  2   | Rol | Escriban aquí su respuesta. | Pantalla, billetera, red, etc. |
|  3   | Rol | Escriban aquí su respuesta. | Pantalla, billetera, red, etc. |
|  4   | Rol | Escriban aquí su respuesta. | Pantalla, billetera, red, etc. |

_(Agreguen los pasos que hagan falta. Si prefieren, inserten aquí un diagrama.)_

---

## 4. Alcance del MVP

> Funcionalidad central separada de la deseable que queda fuera. Justificación de por qué el recorte sigue entregando valor. Extensión: 150–300 palabras en total.

| Dentro del MVP (funcionalidad central) | Fuera del MVP (deseable, para después) |
| -------------------------------------- | -------------------------------------- |
| Escriban aquí su respuesta.            | Escriban aquí su respuesta.            |
| Escriban aquí su respuesta.            | Escriban aquí su respuesta.            |
| Escriban aquí su respuesta.            | Escriban aquí su respuesta.            |

**Por qué el recorte sigue entregando valor:** Escriban aquí su respuesta.

---

## 5. Lean Canvas

> Lienzo de una página con el modelo del producto. Extensión: enlace (obligatorio).

**Enlace al Lean Canvas (obligatorio):** [Lean Canvas del proyecto](https://escriban-aqui-el-enlace)

El lienzo debe cubrir: problema, segmento de usuarios, propuesta de valor única, solución, canales, métricas clave, ventaja diferencial y estructura de costos e ingresos.

---

## 6. Backlog priorizado (Kanban)

> Enlace al tablero en GitHub Projects, construido con las historias priorizadas, en columnas y con criterios de aceptación por tarjeta. Extensión: enlace al tablero (obligatorio).

**Enlace al tablero (obligatorio):** [Tablero Kanban en GitHub Projects](https://github.com/users/darienabdul/projects/6)

---

## 7. Arquitectura inicial

> Cómo se conectan las partes (interfaz, lógica, Stellar) y en qué punto entra la red. Diagrama simple en imagen. Extensión: 150–300 palabras en total.

**Diagrama (imagen o enlace):** Escriban aquí el enlace o inserten la imagen.

|   Capa   | Componente                  | Qué hace                    |
| :------: | --------------------------- | --------------------------- |
| Interfaz | Escriban aquí su respuesta. | Escriban aquí su respuesta. |
|  Lógica  | Escriban aquí su respuesta. | Escriban aquí su respuesta. |
| Stellar  | Escriban aquí su respuesta. | Escriban aquí su respuesta. |

**En qué punto entra la red:** Escriban aquí su respuesta.

---

## 8. Uso de Stellar y justificación

> Qué componentes de Stellar usaría y por qué cada uno. Apoyado en el criterio de pertinencia del Problem Brief. Extensión: 150–300 palabras en total.

**Criterio de pertinencia (del Problem Brief):** Escriban aquí el criterio en el que se apoyan.

| Componente de Stellar       | Para qué lo usamos          | Por qué ese y no otra alternativa |
| --------------------------- | --------------------------- | --------------------------------- |
| Escriban aquí su respuesta. | Escriban aquí su respuesta. | Escriban aquí su respuesta.       |
| Escriban aquí su respuesta. | Escriban aquí su respuesta. | Escriban aquí su respuesta.       |
