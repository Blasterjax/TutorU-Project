# TutorU: Plataforma de Gestión y Coordinación de Tutorías Estudiantiles

Información institucional de la iniciativa:
* **Caso de Estudio:** Caso 03 — Plataforma de tutorías entre estudiantes
* **Entidad Cliente:** Programa de Permanencia Académica — Institución Universitaria de Envigado (IUE)
* **Curso Académico:** IF2008 Ingeniería de Software — Grupo 600
* **Período Lectivo:** Semestre 2026-2

---

## 1. Descripción General

TutorU es una iniciativa de software orientada a estructurar, coordinar y optimizar los procesos de acompañamiento y soporte académico entre pares estudiantiles en la Institución Universitaria de Envigado (IUE), bajo el patrocinio del Programa de Permanencia Académica.

El propósito central del proyecto es transformar un proceso de coordinación tradicionalmente manual, informal y descentralizado en una plataforma centralizada y eficiente, facilitando el encuentro oportuno entre estudiantes tutores y solicitantes, asegurando claridad en los temas de estudio y proveyendo trazabilidad formal para el seguimiento institucional.

---

## 2. Contexto y Formulación del Problema

### 2.1 Contexto
El Programa de Permanencia Académica de la IUE implementa estrategias orientadas a mitigar los índices de deserción estudiantil y fortalecer las competencias en asignaturas de alta exigencia académica. No obstante, la gestión operativa de las tutorías se efectúa actualmente de forma manual mediante intercambios individuales de mensajes a través de aplicaciones de mensajería y redes sociales. Esta dinámica carece de un canal centralizado que consolide la oferta docente estudiantil, los horarios habilitados y el control de cumplimiento.

### 2.2 Problema Central
En la Institución Universitaria de Envigado, los estudiantes que buscan o imparten tutorías experimentan dificultades operativas para coordinar sesiones de apoyo académico, debido a que la solicitud y confirmación se realiza mediante mensajes individuales no estandarizados, sin visibilidad sobre los horarios disponibles ni especificación rigurosa del tema requerido.

Esta situación ocasiona:
* **Colisiones de horario y reservas duplicadas:** Solapamiento de citas para un mismo tutor debido a la falta de concurrencia y validación en tiempo real.
* **Tutorías desarticuladas:** Sesiones poco productivas por falta de delimitación previa de los contenidos o dudas específicas del solicitante.
* **Falta de oportunidad:** Demoras en la confirmación de tutorías en fechas críticas previas a evaluaciones académicas.
* **Ausencia de trazabilidad institucional:** Imposibilidad por parte del Programa de Permanencia Académica de verificar si las sesiones programadas fueron efectivamente impartidas y bajo qué condiciones.

---

## 3. Objetivos del Proyecto

### 3.1 Objetivo General
Diseñar un prototipo navegable de una plataforma de tutorías entre estudiantes que permita coordinar la oferta, solicitud y confirmación de sesiones de apoyo académico, facilitando el encuentro oportuno entre tutores y estudiantes en la Institución Universitaria de Envigado.

### 3.2 Objetivos Específicos
1. **Modelar la estructura de datos y reglas de negocio:** Establecer los esquemas de entidades y restricciones requeridas para administrar ofertas de tutoría, franjas de disponibilidad horaria y solicitudes de servicio.
2. **Definir especificaciones funcionales y de calidad:** Documentar los requisitos funcionales y no funcionales indispensables para agendar, confirmar, reprogramar y cancelar sesiones, garantizando la prevención transaccional de reservas duplicadas.
3. **Representar analíticamente los procesos de usuario:** Construir modelos conceptuales, casos de uso e historias de usuario que reflejen fielmente las necesidades operativas de estudiantes, tutores y la coordinación académica.
4. **Desarrollar la interfaz y prototipado navegable:** Elaborar wireframes estructurales y un prototipo interactivo integral que permita recorrer el flujo operativo completo de extremo a extremo.
5. **Validar la solución con escenarios de prueba:** Evaluar la pertinencia y robustez del prototipo mediante un banco de escenarios de verificación acordados con el cliente y el equipo docente.

---

## 4. Alcance del Sistema

### 4.1 Capacidades Incluidas
* **Catálogo de oferta académica:** Publicación y categorización de tutorías por facultad, programa, asignatura y temas puntuales.
* **Gestión de disponibilidad:** Definición y actualización de franjas horarias por parte de los estudiantes tutores.
* **Ciclo de agendamiento:** Módulo de solicitud, aprobación, reprogramación concertada y cancelación de tutorías.
* **Prevención de colisiones:** Control transaccional y reglas de validación para evitar solapamientos o reservas dobles.
* **Constancia de realización:** Registro de cierre y verificación de ejecución efectiva al culminar cada sesión.
* **Monitoreo institucional:** Vistas de consulta de tutorías activas, completadas e indicadores agregados para la coordinación del programa.

### 4.2 Exclusiones Expresas
Con el objetivo de blindar el alcance académico y asegurar la viabilidad del proyecto, se definen las siguientes exclusiones:
* **Sin videollamadas integradas:** La plataforma no aloja un motor de videoconferencia interno; en modalidad virtual, gestiona enlaces a servicios externos (Microsoft Teams, Google Meet).
* **Sin acceso a notas o calificaciones institucionales:** No se interactúa con bases de datos confidenciales ni historiales académicos oficiales.
* **Sin pasarelas de pago o transferencias económicas:** El servicio de tutorías es de naturaleza formativa e institucional; no contempla transacciones monetarias ni tarifas.
* **Sin diagnósticos académicos o psicológicos automatizados:** La plataforma se enfoca exclusivamente en la logística y gestión del apoyo entre pares.

---

## 5. Enfoque Metodológico de Desarrollo

El proyecto se rige por un enfoque metodológico **Híbrido: Incremental con prácticas ágiles**, justificado técnicamente en la Matriz Comparativa de Procesos:

* **Dimensión Incremental:** Las capacidades funcionales del alcance han sido descompuestas en módulos independientes (oferta, disponibilidad, agendamiento, registro y reportería), facilitando su construcción progresiva e integración continua conforme a las etapas del semestre académico.
* **Dimensión Ágil:** Dado que los requisitos detallados y las reglas de negocio específicas se descubren y refinan a lo largo de las sesiones de interacción con los interesados, se aplican ciclos cortos de retroalimentación semanal para ajustar el backlog sin generar reprocesos estructurales.

---

## 6. Arquitectura y Estructura del Repositorio

El repositorio adopta una jerarquía estandarizada de 7 directorios para asegurar la trazabilidad documental y técnica a lo largo del ciclo de vida del desarrollo:

| Directorio | Propósito y Contenido | Estado Actual |
| :--- | :--- | :--- |
| `00_Gestion/` | Plan de gestión de la iniciativa, actas de acuerdos, cronograma, estructura WBS y matriz RACI. | Completado (Versión 2.0) |
| `01_Iniciativa/` | Ficha de estructuración de iniciativa v0.1 con formulación del problema, interesados y alcance. | Completado (Versión 0.1) |
| `02_Proceso/` | Matriz comparativa de procesos de software y fundamentación técnica del enfoque híbrido. | Completado (Versión 1.0) |
| `03_Requisitos/` | Plan de elicitación, especificación de requisitos (RF/RNF), historias de usuario y matriz de trazabilidad. | Programado (Etapa 2) |
| `04_Modelos/` | Modelos conceptuales, diagramas de clases, casos de uso, diagramas de actividades y estados del sistema. | Programado (Etapa 3) |
| `05_Prototipo/` | Wireframes de baja fidelidad, guía de estilos, componentes de interfaz y prototipo navegable. | Programado (Etapa 4) |
| `06_Evidencias/` | Presentaciones oficiales de sustentación, actas de validación y registros de avance de tablero. | Completado (Seguimiento 1) |

---

## 7. Equipo de Trabajo y Asignación de Roles

| Integrante | Rol en el Proyecto | Responsabilidades Principales | Artefactos a Cargo |
| :--- | :--- | :--- | :--- |
| **Juan José Montoya García** | Líder de Equipo | Coordinación operativa, seguimiento del cronograma, actas de trabajo, matriz de responsabilidades y consolidación del Plan de Gestión. | `E03` |
| **Samuel Gómez Hernández** | Analista de Requisitos e Interesados | Conducción de la elicitación, caracterización de interesados, facilitación del tablero Kanban y control de flujo de trabajo. | `E01`, `E05` |
| **Sebasthian Calderón García** | Responsable de Modelado y Documentación | Redacción y mantenimiento de la Ficha de Iniciativa, elaboración de la Matriz Comparativa de Procesos y aseguramiento de coherencia documental. | `E01`, `E02` |
| **Samuel Cortés Guirales** | Responsable de Prototipado y Validación Técnica | Administración técnica del repositorio en GitHub, gestión de riesgos de arquitectura, diseño de material de sustentación y desarrollo de prototipos. | `E04`, `E06` |

---

## 8. Políticas de Gobernanza y Control de Versiones

### 8.1 Estrategia de Ramas (GitFlow Simplificado)
* `main`: Rama protegida destinada exclusivamente a versiones definitivas, consolidadas y aprobadas para evaluación formal.
* `develop`: Rama central para la integración continua de artefactos de trabajo aprobados.
* `docs/*`: Ramas secundarias destinadas a la redacción, edición y control de calidad de la documentación formal.
* `feat/*`: Ramas secundarias para el diseño de componentes, maquetación de pantallas y código de prototipado.

### 8.2 Estándar de Commits Semánticos
Los registros de confirmación en Git deben ser atómicos, utilizar verbos en imperativo y hacer referencia explícita al identificador de la tarea del desglose analítico (WBS):

```text
[ID_Tarea] [tipo]: [descripción en imperativo]
```

* **Tipos válidos:** `feat` (funcionalidad), `fix` (corrección), `docs` (documentación), `style` (formato), `refactor` (reestructuración), `chore` (mantenimiento o configuración).
* **Ejemplo estándar:** `T06 docs: actualizar documentacion tecnica del repositorio y estandarizar estructura`

### 8.3 Gestión Operativa del Tablero (Kanban)
* **Herramienta oficial:** GitHub Projects integrado al repositorio institucional.
* **Columnas de flujo:** `Backlog` -> `Ready (Listo)` -> `In Progress (En curso)` -> `Review / QA (En revisión)` -> `Done (Hecho)`.
* **Límite de Trabajo en Proceso (WIP):** Se define una política restrictiva de un máximo de **2 tareas simultáneas** por equipo en la columna *In Progress* y máximo **2 tareas** en *Review*, minimizando la multitarea y mitigando cuellos de botella.
* **Criterio de Terminado (Definition of Done - DoD):** Ningún entregable o tarea puede ser promovido al estado *Done* sin cumplir con la revisión cruzada obligatoria efectuada por un compañero distinto al responsable de ejecución y la verificación de trazabilidad frente a los lineamientos de la asignatura.

