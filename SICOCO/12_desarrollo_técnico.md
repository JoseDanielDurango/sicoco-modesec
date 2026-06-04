# Documentación Técnica: SICOCO (Sintetizador de Co-creación Colaborativa)

### 1. Objetivo del Sistema

El objetivo de **SICOCO** es servir como una herramienta digital de procesamiento de texto basada en **Inteligencia Artificial** diseñada para analizar, clasificar y resumir transcripciones de chats y foros de trabajo grupal. El sistema busca transformar la opacidad de las discusiones asíncronas en un proceso transparente de co-creación, permitiendo a los estudiantes visualizar cómo colaboran y facilitando el seguimiento docente bajo la metodología **MODESEC**.

### 2. Perfiles de Usuario

* **Estudiante (Usuario Principal):** Responsable de ingresar los historiales de chat, visualizar los resúmenes, gestionar sus tareas asignadas y evaluar la utilidad de la herramienta.
* **Docente / Evaluador:** Vinculado a asignaturas para supervisar los niveles de participación, validar consensos alcanzados por los equipos y calificar la fidelidad técnica del sistema.
* **Administrador:** Encargado de la gestión de roles, mantenimiento técnico y seguridad global de la infraestructura de datos.

### 3. Funcionalidades del Software (MVP)

El despliegue final se ha definido como una **extensión de navegador** (compatible con navegadores basados en Chromium) para facilitar la captura e importación directa de datos desde plataformas de mensajería en sus versiones web.

#### A) Módulo de Captura y Procesamiento (IA)

* **Captura Directa e Ingreso de Historiales:** Capacidad para capturar y extraer mensajes directamente desde la interfaz web de plataformas de mensajería (WhatsApp Web, Discord Web, Teams Web) leyendo el DOM de la pestaña activa en el navegador. Asimismo, permite la carga de archivos de chat exportados (txt, csv, JSON) de forma asíncrona.
* **Motor de SICOCO:** Consumo de APIs de IA generativa (Gemini/OpenAI) mediante una **Ingeniería de Prompts** robusta para minimizar alucinaciones.
* **Categorización Pedagógica:** Identificación automática de cuatro ejes fundamentales:
  * **Acuerdos:** Puntos de consenso y decisiones tomadas.
  * **Desacuerdos:** Posturas encontradas y debates en curso.
  * **Dudas:** Interrogantes sin resolver al finalizar la sesión.
  * **Tareas (To-Do):** Compromisos, responsables y fechas límite.

#### B) Visualización y Dashboard (GUI)

* **Línea de Tiempo de Co-creación:** Representación visual de cómo evolucionaron las ideas y los hitos cronológicos del equipo.
* **Identificación de Autores:** Reconocimiento de quién aportó cada idea o solución para validar la participación individual.
* **Estilos de Resumen:** Opción de elegir entre un tono "Serio" (para informes) o "Rápido" (para seguimiento directo).
* **Edición Manual:** Permite al estudiante corregir errores del resumen generado antes del almacenamiento final.

### 4. Arquitectura de Datos (Modelo Relacional)

El sistema se organiza en **6 dominios funcionales** con un total de **19 entidades**:

* **Dominio Técnico-Académico:** Tablas de *Estudiante*, *Profesor*, *Curso*, *Equipo* y *Miembro_Equipo* para gestionar identidades y jerarquías.
* **Sesiones de Trabajo:** *Sesion_Trabajo*, *Registro_Chat* y *Mensaje_Original* para auditar el insumo crudo.
* **Procesamiento IA:** *Configuracion_Prompt* y *Resumen_Generado* para manejar la lógica del motor de IA.
* **Pilares de Información:** Entidades específicas para *Acuerdo_Equipo*, *Desacuerdo*, *Duda_Abierta* y *Tarea_Asignada*.
* **Mapeo de Co-creación:** *Momento_Clave_Chat* y la tabla recursiva *Conexion_Idea* para construir el grafo de interacciones.
* **Evaluación y Calidad:** *Control_Calidad_Bot*, *Evaluacion_UX* y *Encuesta_Piloto* para medir el impacto educativo y técnico.

### 5. Flujos Críticos

1. **Procesamiento de Chat:** El estudiante captura el chat vía extensión -> La IA categoriza mensajes -> Se genera un resumen estructurado en el Dashboard.
2. **Seguimiento Docente:** El docente accede al curso -> Revisa los acuerdos y tareas de los equipos -> Evalúa la fidelidad del resumen frente al chat original.

### 6. Requisitos No Funcionales y Seguridad

* **Privacidad:** Blindaje lógico de accesos; los estudiantes solo ven material de sus equipos respectivos.
* **Auditoría:** Campos obligatorios de `Created_At` y `Updated_At` en todas las tablas para trazabilidad de cambios.
* **Integridad:** Uso de UUIDs para identificadores sensibles y encriptación de contraseñas mediante hash.
* **Escalabilidad:** Desacoplamiento de remitentes (Alias) para permitir el procesamiento de usuarios externos no registrados en la plataforma.

### 7. Roadmap de Desarrollo (Fases MODESEC)

1. **Diagnóstico:** Definición de competencias y problemas de sobrecarga informativa (Completado).
2. **Diseño Pedagógico y Planificación:** Estructuración de categorías (Acuerdos, Tareas, etc.), entrevistas de requerimientos e historias de usuario (Completado).
3. **Diseño Computacional y Técnico:** Modelos de entidad-relación (MER), diseño del desarrollo técnico y arquitectura del MVP (Completado).
4. **Producción y Desarrollo:** Programación del frontend (extensión), backend e ingeniería de prompts.
5. **Evaluación:** Pruebas de precisión técnica, usabilidad (UX) y utilidad educativa.
6. **Implementación:** Programa piloto en cursos reales de la Universidad de Córdoba.
