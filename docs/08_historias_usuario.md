Matriz de Historias de Usuario - Proyecto SICOCO

**Basado en Arquitectura de Datos y Metodología MODESEC**
# **ZONA 1: Usuarios, Roles y Organización (PER)**
Entidades: Estudiante, Profesor, Administrador, Curso y Equipo.

|**ID**|**Historia (Como / Quiero / Para)**|**Valor**|**Prioridad**|**Dependencias**|**Criterios de aceptación**|
| :- | :- | :- | :- | :- | :- |
|PER-01|Como estudiante, quiero registrarme con mi ID, programa y semestre para ser identificado en el sistema.|Alta|Must|Ninguna|Dado que ingreso mis datos académicos. Cuando guardo Entonces se crea el registro en la entidad Estudiante.|
|PER-02|Como docente, quiero vincularme a una asignatura para supervisar los grupos de trabajo.|Alta|Must|PER-01|Dado que el usuario tiene rol Docente. Cuando selecciona una asignatura Entonces queda asignado como mentor del curso.|
|PER-03|Como usuario, quiero recuperar mi contraseña mediante correo para no perder acceso a mi cuenta.|Media|Should|PER-01|Dado un correo registrado. Cuando solicita recuperación Entonces se envía un link temporal de acceso.|
|PER-04|Como integrante de equipo, quiero ser vinculado a un ID\_Equipo para trabajar colaborativamente.|Alta|Must|PER-01|Dado un grupo creado. Cuando el admin me añade Entonces mi ID se relaciona con el ID\_Equipo.|

# **ZONA 2: Entradas y Sesiones de Trabajo (SES)**
Manejo de la entidad Reunión, Archivo\_Chat y Mensajes individuales.

|**ID**|**Historia (Como / Quiero / Para)**|**Valor**|**Prioridad**|**Dependencias**|**Criterios de aceptación**|
| :- | :- | :- | :- | :- | :- |
|SES-01|Como estudiante, quiero crear una Sesión de Trabajo con fecha y hora para iniciar la co-creación.|Alta|Must|PER-04|Dado un ID\_Equipo. Cuando se abre la sesión Entonces se genera el registro en la entidad Sesion\_Trabajo.|
|SES-02|Como estudiante, quiero subir un archivo .txt o .csv para que el sistema administre el archivo físico.|Alta|Must|SES-01|Dado un archivo de chat. Cuando se sube Entonces se guarda la ruta, tamaño y fecha en la tabla Archivo.|
|SES-03|Como sistema, quiero separar los mensajes individuales (Cuerpo y Autor) para analizarlos por separado.|Alta|Must|SES-02|Dado un archivo cargado. Cuando se procesa Entonces cada línea se guarda con su ID\_Autor y Marca\_Tiempo.|
|SES-04|Como usuario, quiero ver el historial de archivos subidos por sesión para evitar duplicar información.|Media|Should|SES-02|Dado una sesión activa. Cuando consulto archivos Entonces el sistema lista los nombres y fechas de carga.|

# **ZONA 3: Motor de IA y Procesamiento (IA)**
Uso de Ingeniería de Prompts y categorización (Acuerdos, Tareas, Dudas).

|**ID**|**Historia (Como / Quiero / Para)**|**Valor**|**Prioridad**|**Dependencias**|**Criterios de aceptación**|
| :- | :- | :- | :- | :- | :- |
|IA-01|Como sistema, quiero categorizar mensajes en Acuerdos, Dudas y Tareas para estructurar la síntesis.|Alta|Must|SES-03|Dado el texto del chat. Cuando la IA procesa Entonces asigna una categoría a cada punto clave.|
|IA-02|Como sistema, quiero extraer tareas (To-Do) con descripción y responsable para organizar el trabajo.|Alta|Must|IA-01|Dado un compromiso detectado. Cuando la IA lo procesa Entonces se crea una fila en la tabla Tarea con su Responsable.|
|IA-03|Como estudiante, quiero que la IA identifique dudas sin resolver para que el grupo las retome luego.|Media|Should|IA-01|Dado una pregunta sin respuesta en el chat. Cuando termina el análisis Entonces se lista en Dudas\_Pendientes.|
|IA-04|Como sistema, quiero detectar contradicciones en el chat para avisar al grupo sobre posibles malentendidos.|Baja|Could|IA-01|Dado dos mensajes opuestos. Cuando se hace la síntesis Entonces se añade una nota de "Conflicto detectado".|

# **ZONA 4: Visualización y Línea de Tiempo (GUI)**
Entidades de Mapeo de Co-creación y visualización de hitos.

|**ID**|**Historia (Como / Quiero / Para)**|**Valor**|**Prioridad**|**Dependencias**|**Criterios de aceptación**|
| :- | :- | :- | :- | :- | :- |
|GUI-01|Como estudiante, quiero ver una línea de tiempo con los hitos del chat para entender la evolución de las ideas.|Alta|Should|IA-01|Dado el resumen generado. Cuando cargo la vista Entonces se muestran los elementos de la tabla Hito\_Cronologico.|
|GUI-02|Como usuario, quiero ver la interconexión entre una idea y su solución para validar el aporte de cada uno.|Media|Should|GUI-01|Dado un acuerdo. Cuando pulso en él Entonces el sistema resalta los mensajes de origen (Contribución\_ID).|
|GUI-03|Como estudiante, quiero elegir entre un estilo de resumen Serio o Rápido según mi necesidad.|Media|Could|IA-04|Dado el resumen finalizado. Cuando selecciono estilo Entonces la visualización cambia el nivel de detalle.|
|GUI-04|Como estudiante, quiero ver el resumen dividido por categorías para leer solo lo que me interesa.|Alta|Must|IA-01|Dado el resumen generado. Cuando se carga el dashboard Entonces aparecen pestañas por cada categoría.|

# **ZONA 5: Evaluación y Seguridad (EVA)**
Control de Calidad, Auditoría y Privacidad (Created\_At, Updated\_At).

|**ID**|**Historia (Como / Quiero / Para)**|**Valor**|**Prioridad**|**Dependencias**|**Criterios de aceptación**|
| :- | :- | :- | :- | :- | :- |
|EVA-01|Como docente, quiero calificar la fidelidad del resumen (1-10) para evaluar el desempeño técnico.|Media|Should|GUI-01|Dado un resumen revisado. Cuando el docente califica Entonces se guarda en Control\_Calidad\_IA.|
|EVA-02|Como estudiante, quiero reportar un error en el resumen para que el sistema aprenda de la corrección.|Baja|Could|GUI-01|<p>Dado un texto incorrecto. Cuando se marca como "Error" Entonces se guarda el registro para re-entrenamiento.</p><p></p>|
|EVA-03|Como administrador, quiero un historial de modificaciones para auditar quién cambió un resumen.|Alta|Must|GUI-01|Dado un cambio en los datos. Cuando se guarda Entonces se actualiza el campo Updated\_At y el ID\_Editor.|
|EVA-04|Como sistema, quiero restringir el acceso a usuarios no autorizados para proteger la privacidad del grupo.|Alta|Must|PER-04|Dado un intento de consulta anónima. Cuando se valida el rol Entonces el sistema bloquea la vista si no pertenece al equipo.|

