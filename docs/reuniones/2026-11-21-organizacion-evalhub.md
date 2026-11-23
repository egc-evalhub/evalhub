# Registro de organización y planificación — EvalHub

**Fecha de referencia:** 21 de noviembre de 2026  
**Proyecto:** EvalHub — EGC 2026/2027, Universidad de Sevilla  
**Responsable de documentación:** Manuel Rivera Gálvez (Project Manager)  
**Integrantes del equipo:** Manuel Rivera Gálvez, Iván Jesús Sevillano Plaza y Francisco Javier Herrera de Isla

## 1. Objetivos de la planificación

1. Revisar el acta fundacional y las responsabilidades del equipo.
2. Analizar el alcance funcional y técnico de EvalHub.
3. Organizar los Work Items y distribuir las subtareas.
4. Establecer la gestión del repositorio y la documentación.
5. Preparar el seguimiento del 23 de noviembre de 2026.

## 2. Revisión del acta fundacional

El acta fundacional v3 establece los roles y responsabilidades siguientes:

- **Manuel Rivera Gálvez — Project Manager:** planificación, reparto de tareas, convocatoria y documentación de reuniones, mantenimiento de GitHub Projects y comunicación con el tutor.
- **Iván Jesús Sevillano Plaza — Calidad y DevOps:** revisión de cambios, pruebas automatizadas, CI/CD y entornos de desarrollo y producción.
- **Francisco Javier Herrera de Isla — Gestión de configuración:** aplicación de EGCFlow, ramas, integración, etiquetas y entregas.

El canal habitual de coordinación es WhatsApp y el previsto para reuniones telemáticas es Microsoft Teams. Las decisiones relevantes y su trazabilidad deben quedar documentadas en el repositorio.

## 3. Análisis general de EvalHub

EvalHub permitirá gestionar y compartir datasets para evaluar modelos de lenguaje, especialmente ficheros **JSONL** con casos que incluyen `id`, `input` y `expected_output`. El trabajo comprende validación y subida de archivos, metadatos específicos, previsualización, estadísticas, búsqueda, integración con Fakenodo y versionado.

**Cuestión pendiente de confirmar con el tutor:** el WI-newdataset original (#178 de EGCETSII/uvlhub) requiere conservar la funcionalidad UVL existente mientras se añade el nuevo tipo de dataset. El acta fundacional v3 describe su sustitución; hasta recibir una aclaración, conviene evitar cambios que eliminen soporte UVL.

## 4. Distribución de trabajo en GitHub Issues

Los siguientes Issues están creados en el repositorio [`egc-evalhub/evalhub`](https://github.com/egc-evalhub/evalhub). El reparto reflejado aquí corresponde a la planificación del proyecto.

| Issue | Trabajo | Responsable |
|---|---|---|
| [#1](https://github.com/egc-evalhub/evalhub/issues/1) | Adaptación de UVLHub a EvalHub (WI-newdataset) | Todo el equipo |
| [#2](https://github.com/egc-evalhub/evalhub/issues/2) | Fakenodo | Manuel |
| [#3](https://github.com/egc-evalhub/evalhub/issues/3) | Major versioning | Francisco Javier |
| [#4](https://github.com/egc-evalhub/evalhub/issues/4) | Viewing versions | Manuel |
| [#5](https://github.com/egc-evalhub/evalhub/issues/5) | Advanced search | Iván |
| [#6](https://github.com/egc-evalhub/evalhub/issues/6) | Análisis de arquitectura y componentes | Todo el equipo |
| [#7](https://github.com/egc-evalhub/evalhub/issues/7) | Modelos de datos y migraciones | Francisco Javier |
| [#8](https://github.com/egc-evalhub/evalhub/issues/8) | Validación y subida de JSONL | Manuel |
| [#9](https://github.com/egc-evalhub/evalhub/issues/9) | Formularios y vistas de datasets | Iván |
| [#10](https://github.com/egc-evalhub/evalhub/issues/10) | Exploración, descargas y estadísticas | Iván |
| [#11](https://github.com/egc-evalhub/evalhub/issues/11) | Seeders y pruebas de regresión | Todo el equipo |
| [#12](https://github.com/egc-evalhub/evalhub/issues/12) | Organización de la documentación del proyecto | Manuel |

Las tareas #6 a #11 desglosan el WI-newdataset (#1). El Issue #12 agrupa la preparación de la carpeta `docs/`, el acta fundacional, la documentación de planificación y los registros de reuniones y decisiones.

## 5. Dependencias y coordinación

- **#2 → #3:** Fakenodo sirve para probar las operaciones de publicación y versionado con DOI.
- **#3 → #4:** la visualización de versiones requiere disponer de la lógica de versionado principal.
- **#1 → #5, #9 y #10:** los metadatos y modelos de EvalHub condicionan la búsqueda, los formularios y la exploración.
- **#6 → #7 y #8:** el análisis de arquitectura permite delimitar los modelos y la validación.
- **#11:** las pruebas deben comprobar tanto el nuevo soporte JSONL como las funcionalidades UVL que deban mantenerse.

## 6. Organización del repositorio

Se utiliza la organización de GitHub `egc-evalhub` y el repositorio `evalhub`. Las ramas permanentes son:

- **`main`:** entregas estables.
- **`trunk`:** integración del trabajo del equipo.

De acuerdo con EGCFlow, las ramas de tarea salen de `trunk`, se vinculan a una incidencia y se revisan por otro integrante antes de integrarse. Se emplean commits trazables y se evita trabajar directamente sobre `main` o `trunk`.

Las incidencias se supervisan con GitHub Projects mediante los estados **Todo**, **In Progress**, **In Review** y **Done**. El estado actualizado de cada tarea se consulta allí.

La documentación se centraliza en `docs/`, con secciones para acta fundacional, reuniones, plantillas, planificación y decisiones. El Issue #12 recoge esta labor.

## 7. Acciones planificadas para el seguimiento del 23 de noviembre

| Acción | Responsable | Fecha objetivo |
|---|---|---|
| Verificar el tablero y las asignaciones de Issues | Manuel | 22/11/2026 |
| Organizar y versionar los documentos del proyecto (`#12`) | Manuel | 22/11/2026 |
| Comprobar la política de ramas y la trazabilidad EGCFlow | Francisco Javier | 22/11/2026 |
| Revisar las pruebas y los workflows existentes | Iván | Por concretar |
| Preparar una explicación del estado de tareas y dependencias | Todo el equipo | 23/11/2026 |

Estas fechas son objetivos de planificación, no certificaciones de ejecución. Los avances efectivos se registrarán en GitHub Issues, commits y documentación asociada.

## 8. Cuestiones pendientes

- Confirmar con José Manuel Sánchez Ruiz el alcance de la compatibilidad con UVL.
- Acordar la secuencia de implementación de las funcionalidades dependientes.
- Verificar el funcionamiento local y el estado de CI/CD.
- Concretar la siguiente reunión y documentar, en su caso, los acuerdos adoptados.

---

**Nota de trazabilidad:** este documento recoge la planificación y la distribución de trabajo preparadas para EvalHub. No constituye por sí solo acreditación de asistencia a una reunión; las actas de reuniones efectivamente celebradas se conservarán por separado en `docs/reuniones/`.
