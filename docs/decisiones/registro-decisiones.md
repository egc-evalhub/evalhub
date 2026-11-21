# Registro de decisiones y cuestiones pendientes — EvalHub

El registro separa **acuerdos recogidos en el acta fundacional** de **propuestas de organización posteriores**. No atribuye a una reunión hechos no acreditados.

## Acuerdos documentados en el acta fundacional v3

### DEC-001 — Dominio de EvalHub
- **Fuente:** acta fundacional v3, apartado 2.
- **Contenido:** plataforma para compartir datasets de evaluación de modelos de lenguaje con ficheros JSONL y metadatos específicos.
- **Pendiente:** confirmar con el tutor cómo compatibilizar el texto del acta con la obligación de mantener UVL en el WI original #178.

### DEC-002 — Roles del equipo
- **Fuente:** acta fundacional v3, apartado 3.
- **Contenido:** Manuel (Project Manager), Iván (calidad y DevOps), Francisco Javier (gestión de configuración); todos programan.

### DEC-003 — Política EGCFlow
- **Fuente:** acta fundacional v3, apartado 5.
- **Contenido:** `main` para entregas, `trunk` para integración; ramas de tarea desde `trunk`, revisión de un compañero e integración con `git merge --no-ff` sin Pull Requests internos.

### DEC-004 — Gestión del trabajo
- **Fuente:** acta fundacional v3, apartado 7.
- **Contenido:** GitHub Issues y tablero GitHub Projects; WI comunes #178 y #177, altos #196 y #197, medio #194.

## Organización preparada posteriormente (pendiente de ratificación formal)

### PROP-001 — Subdivisión de WI-newdataset
- **Referencia:** Issues del equipo #6–#11.
- **Propuesta:** dividir el trabajo en arquitectura, modelos, validación JSONL, interfaz, exploración y pruebas.
- **Pendiente:** confirmar reparto y equilibrar especialmente la carga de Iván.

### PROP-002 — Estructura documental
- **Propuesta:** centralizar documentos bajo `docs/`, separar plantillas de actas celebradas y mantener referencias a GitHub Issues.
- **Pendiente:** revisión del equipo e integración según EGCFlow.

## Plantilla para nuevas decisiones

### DEC-XXX — [Título]
- **Fecha:** [DD/MM/AAAA]
- **Participantes:** [Nombres]
- **Contexto:** [Necesidad o problema]
- **Decisión:** [Acuerdo concreto]
- **Justificación:** [Motivos]
- **Consecuencias:** [Impacto]
- **Issues relacionados:** [Enlaces]
- **Estado:** Propuesta / Vigente / Sustituida
