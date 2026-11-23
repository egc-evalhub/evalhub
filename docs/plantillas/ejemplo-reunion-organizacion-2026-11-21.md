# EJEMPLO SIMULADO — Reunión de organización de EvalHub

> **DOCUMENTO DE EJEMPLO.** Esta reunión es ficticia y **no debe presentarse como acta de una reunión celebrada**. El texto aprovecha tareas y decisiones documentadas en GitHub y la planificación de este proyecto. Si el equipo celebra una reunión equivalente, hay que escribir una nueva acta con los hechos efectivamente confirmados.

**Fecha ficticia:** 21/11/2026  
**Hora:** no establecida  
**Modalidad sugerida:** Microsoft Teams  
**Redactaría:** Manuel Rivera Gálvez, Project Manager

## 1. Asistencia (simulada)

- Manuel Rivera Gálvez.
- Iván Jesús Sevillano Plaza.
- Francisco Javier Herrera de Isla.

## 2. Orden del día propuesto

1. Revisión del alcance de EvalHub y del repositorio base UVLHub.
2. Organización de los Work Items y sus dependencias.
3. Distribución del WI-newdataset en subtareas.
4. Preparación del seguimiento del 23/11/2026.

## 3. Resumen de los asuntos para debatir

**Alcance técnico.** EvalHub se orienta a datasets JSONL para evaluar modelos de lenguaje, con metadatos de tarea, idioma, métrica y categorías, validación, búsqueda, descarga y versionado. Conviene contrastar el acta del equipo con el enunciado original del WI-newdataset, que pide conservar el soporte UVL mientras se introduce un nuevo tipo de dataset.

**Control del trabajo.** En GitHub están creados los Issues #1 a #11. `main` se reserva a las entregas estables y `trunk` a la integración. Las tareas se revisarán en el tablero de GitHub Projects.

**Dependencias.** La visualización de versiones (#4) depende del versionado principal (#3). Fakenodo (#2) proporciona el servicio de pruebas que necesita el versionado. Las subtareas de modelos, subida, vistas y pruebas deben coordinarse.

## 4. Reparto que se revisaría

| Issue | Trabajo | Responsable previsto |
|---|---|---|
| #1 | Adaptación de UVLHub a EvalHub | Equipo completo |
| #2 | Fakenodo | Manuel |
| #3 | Major versioning | Francisco Javier |
| #4 | Viewing versions | Manuel |
| #5 | Advanced search | Iván |
| #6 | Análisis de arquitectura | Equipo completo |
| #7 | Modelos y migraciones | Francisco Javier |
| #8 | Validación y subida de JSONL | Manuel |
| #9 | Formularios y vistas | Iván |
| #10 | Exploración, descargas y estadísticas | Iván |
| #11 | Seeders y pruebas | Equipo completo |

## 5. Próximas acciones propuestas

- Comprobar propietarios, prioridades, dependencias y estados del tablero.
- Acordar y documentar la distribución del trabajo de #1.
- Crear ramas de tarea desde `trunk` y enlazar sus commits a los Issues.
- Identificar evidencias verificables para el seguimiento del 23/11/2026.
- Confirmar con el tutor las discrepancias entre el alcance de #178 y el acta fundacional.

**Próxima reunión:** no establecida en este ejemplo.
