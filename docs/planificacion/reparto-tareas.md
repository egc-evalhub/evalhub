# Planificación y reparto de tareas — EvalHub

**Referencia:** acta fundacional v3, GitHub Issues y organización trabajada hasta el 21/11/2026.  
**Seguimiento:** [Issues del equipo](https://github.com/egc-evalhub/evalhub/issues).

## Work Items principales

| Issue del equipo | WI original | Trabajo | Responsable según el acta |
|---|---|---|---|
| [#1](https://github.com/egc-evalhub/evalhub/issues/1) | [#178](https://github.com/EGCETSII/uvlhub/issues/178) | Adaptación UVLHub a EvalHub | Los tres |
| [#2](https://github.com/egc-evalhub/evalhub/issues/2) | [#177](https://github.com/EGCETSII/uvlhub/issues/177) | Fakenodo | Manuel |
| [#3](https://github.com/egc-evalhub/evalhub/issues/3) | [#196](https://github.com/EGCETSII/uvlhub/issues/196) | Major versioning | Francisco Javier |
| [#4](https://github.com/egc-evalhub/evalhub/issues/4) | [#197](https://github.com/EGCETSII/uvlhub/issues/197) | Viewing versions | Manuel |
| [#5](https://github.com/egc-evalhub/evalhub/issues/5) | [#194](https://github.com/EGCETSII/uvlhub/issues/194) | Advanced search | Iván |

## Subtareas de WI-newdataset (reparto propuesto)

| Issue | Tarea | Responsable previsto |
|---|---|---|
| [#6](https://github.com/egc-evalhub/evalhub/issues/6) | Análisis de arquitectura y separación de componentes | Los tres |
| [#7](https://github.com/egc-evalhub/evalhub/issues/7) | Modelos y migraciones | Francisco Javier |
| [#8](https://github.com/egc-evalhub/evalhub/issues/8) | Validación y subida JSONL | Manuel |
| [#9](https://github.com/egc-evalhub/evalhub/issues/9) | Formularios de subida y vistas | Iván |
| [#10](https://github.com/egc-evalhub/evalhub/issues/10) | Exploración, descargas y estadísticas | Iván |
| [#11](https://github.com/egc-evalhub/evalhub/issues/11) | Seeders y pruebas de regresión | Los tres |

El reparto de las subtareas refleja la planificación preparada en el tablero; debe ratificarse entre los integrantes antes de presentarlo como acuerdo colectivo. Los estados actuales se consultan en GitHub Projects.

## Dependencias técnicas

- **#4 depende de #3:** visualizar versiones requiere que exista el modelo y flujo de versionado.
- **#3 se apoya en #2:** Fakenodo simula Zenodo para probar versiones y DOI.
- **#7 precede a buena parte de #8, #9 y #10:** la estructura de modelos y migraciones condiciona los demás flujos.
- **#11 comprueba el conjunto:** pruebas y seeders cubren los nuevos flujos y evitan regresiones en UVL.

## Fechas de seguimiento

| Fecha | Hito |
|---|---|
| 09/11/2026 | Acta fundacional |
| 23/11/2026 | Gestión de código fuente e incidencias |
| 30/11/2026 | Pruebas automatizadas y CI/CD |
| 14 y 16/12/2026 | Defensa final |

## Preparación inmediata del 23/11

- Revisar las asignaciones y etiquetas de los Issues #1–#11.
- Mostrar `main`, `trunk` y las ramas de tarea que realmente se hayan creado.
- Aportar commits trazables a las incidencias y revisiones reales, si existen.
- Mostrar el estado del tablero y justificar bloqueos y dependencias.
- Registrar acuerdos reales en el diario del equipo.

## Atención al alcance de #1

El acta v3 describe una sustitución de los modelos UVL por datasets de evaluación. En cambio, la incidencia original #178 exige conservar el soporte UVL y añadir un tipo nuevo. **Conviene aclarar este punto con el tutor** y adaptar el alcance de las tareas a su respuesta.
