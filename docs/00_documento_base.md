# 📖 Documento Base de SICOCO

**Contexto Académico:**
El proyecto **SICOCO (Sintetizador de Co-creación Colaborativa)** nace como una iniciativa de los estudiantes de **8vo semestre** de la **Licenciatura en Informática con énfasis en medios audiovisuales** de la **Universidad de Córdoba**. Desarrollado bajo la materia de **Diseño y Desarrollo de Software Educativo I**, empleando la metodología pedagógica **MODESEC**.

---

## 📝 Descripción del Proyecto

SICOCO es una herramienta digital de procesamiento de texto basada en Inteligencia Artificial diseñada para analizar, clasificar y resumir transcripciones de chats y foros de trabajo grupal. Su propósito no es solo resumir información, sino servir como una guía de apoyo que le permita a los estudiantes visualizar cómo colaboran, fomentando el trabajo en equipo.

---

## ⚠️ El Problema

El entorno de aprendizaje actual exige que los estudiantes trabajen en equipo utilizando herramientas asíncronas y chats de mensajería (WhatsApp, Discord, Teams). Esto genera una **sobrecarga de información**, provocando que valiosas ideas, debates importantes y acuerdos consensuados se pierdan o se olviden en medio de extensas cadenas de mensajes. SICOCO tiene que resolver este problema identificando:
1. 🗣️ **Qué se dice** y los acuerdos alcanzados.
2. 👤 **Quién dio cada idea** para validar participaciones.
3. 🤝 **Cómo el grupo debatió** hasta llegar a la resolución.

---

## 💡 La Solución Propuesta

Desarrollar un Producto Mínimo Viable (cuyo formato de despliegue está sujeto a evaluación técnica y podría ser una app web, un programa local, una extensión, etc.) que permita a los estudiantes ingresar sus historiales de chat grupal y utilizar Inteligencia Artificial para extraer de forma estructurada los puntos más importantes de la discusión, categorizándolos visualmente.

---

## 👥 Usuarios Objetivo

- **🎓 Estudiantes Universitarios y Escolares:** Principales beneficiarios que buscan optimizar su tiempo y no perder el hilo de sus proyectos grupales.
- **👨‍🏫 Docentes / Evaluadores:** Que requieren observar o validar el verdadero nivel de participación, los debates y los consensos a los que llegan los grupos de estudiantes fuera del aula.
- **💼 Equipos de Trabajo General:** Grupos que trabajan de forma remota y necesitan no olvidar las decisiones del proyecto.

---

## 🎯 Objetivos

### Objetivo General
Desarrollar un Producto Mínimo Viable de la herramienta SICOCO que utilice Inteligencia Artificial para resumir chats colaborativos, estructurando la información según la metodología MODESEC para facilitar la asimilación del aprendizaje en estudiantes de educación superior.

### Objetivos Específicos
1. **Clasificar el contenido** extraído en cuatro ejes fundamentales: Acuerdos, Desacuerdos, Tareas (To-Do) y Dudas sin resolver.
2. **Generar un reporte visual y amigable** (Línea de tiempo y Tableros) que permita al estudiante comprender de un solo vistazo el estatus de su proyecto.
3. **Identificar al autor de las ideas** para destacar el aporte de cada persona al trabajo del equipo.
4. **Validar la utilidad educativa** de la herramienta mediante pruebas de campo (usabilidad y fidelidad técnica) en el entorno universitario.

---

## 🏗️ Fundamentación Metodológica Integral (Modelo MODESEC)

La fundamentación metodológica del proyecto SICOCO se basa en la integración sinérgica del modelo **MODESEC** (Modelo de Organización de Estrategias para el Desarrollo de Software Educativo por Competencias). Este marco no se limita a una simple guía instruccional, sino que se constituye como un ecosistema de organización pedagógica orientado específicamente al diseño de software educativo basado en competencias, evidencias de aprendizaje y mediaciones tecnológicas.

1. **La Primacía del Aprendizaje:** SICOCO se concibe como un sistema que transforma la opacidad de los chats grupales en un proceso transparente de co-creación, donde cada algoritmo y línea de código están supeditados a objetivos formativos validados. La tecnología deja de ser el fin para convertirse en el medio que hace tangible el progreso intelectual del equipo.
2. **Principios Orientadores:** El software debe fortalecer la capacidad del estudiante para trabajar de forma colaborativa, identificando acuerdos y resolviendo dudas de manera autónoma. Cada funcionalidad técnica debe generar o procesar una evidencia observable del desempeño del estudiante.
3. **Framework de Ingeniería:** MODESEC permite segmentar el ciclo de vida del software, priorizando requerimientos que generan evidencias de aprendizaje y alineando la arquitectura de datos con los estándares de calidad educativa y técnica.
4. **Dominio Técnico-Académico:** Gestión de identidades, roles (docente/estudiante) y organización de cursos.
5. **Dominio del Procesamiento Pedagógico:** Núcleo de inteligencia donde el motor de IA aplica filtros metodológicos para transformar el contenido desestructurado.
6. **Dominio de Visualización Educativa:** Diseño de la interfaz gráfica (GUI) para presentar mapas de co-creación y líneas de tiempo.
7. **El Motor de IA y MODESEC:** Se emplea una ingeniería de prompts robusta basada en las categorías de MODESEC para identificar evidencias específicas de desempeño, minimizando alucinaciones tecnológicas.

---

## 🗺️ Fases del Proyecto (Enfoque MODESEC)

### 🔍 Fase 1: Diagnóstico (Análisis de Competencias)
En este paso definimos qué debe lograr la persona que usa el sistema y qué problema debe resolver la Inteligencia Artificial. La meta principal es: **“Resumir y analizar lo que el grupo habla al trabajar en equipo, sirviendo como una guía de apoyo”.**

### 🧠 Fase 2: Diseño Pedagógico (Formas de Enseñar)
SICOCO debe ordenar la información de forma clara. En lugar de dar un resumen aburrido, divide las conclusiones en partes clave:
1. ✅ **Acuerdos:** Puntos donde el equipo pensó igual y tomó una decisión.
2. ❌ **Desacuerdos u objeciones:** Opiniones diferentes o debates.
3. ❓ **Dudas sin resolver:** Preguntas que nadie supo responder al terminar la reunión.
4. 📋 **Tareas por hacer:** Próximos pasos a seguir y quién tiene que hacerlos.

El resumen debe mostrar, mediante una **línea de tiempo fácil de leer**, cómo fueron cambiando las ideas principales para demostrar el valor del trabajo en equipo.

### 💻 Fase 3: Diseño Computacional (Arquitectura y Fundamentación Tecnológica)
Este es el plan básico para desarrollar el programa bajo un modelo **MVP (Producto Mínimo Viable)**. 
- **Entrada de Datos (Básica y Segura):** Se proveerá una interfaz sencilla donde el estudiante ingresará el historial exportado de sus chats de trabajo grupal, evitando la complejidad de integraciones en tiempo real (web scraping, bots).
- **El Motor de SICOCO (Procesamiento):** Consumirá APIs de Inteligencias Artificiales generativas de bajo costo o capa gratuita (como Gemini o OpenAI). Se utilizará un sistema robusto de instrucciones estructuradas (**Ingeniería de Prompts**), en lugar de entrenar una IA desde cero (fine-tuning).
- **Pantalla para el Usuario (UI):** Se construirá una interfaz gráfica (Dashboard) estructurada y clara para exponer visualmente los elementos extraídos (autor, tareas pendientes, acuerdos).

### 🛠️ Fase 4: Producción y Desarrollo
Se programará la interfaz donde el usuario cargará su documento y cómo el backend se conecta a la API de IA. 
- **Ingeniería de Prompts:** La parte más crítica será perfeccionar las instrucciones para minimizar alucinaciones y extraer información precisa.
- **Tipos de Textos:** El sistema deberá manejar chats rápidos y cortos (WhatsApp/Telegram) así como foros ordenados y formales, adaptándose al ritmo conversacional.

### 📊 Fase 5: Evaluación (Pruebas de Campo)
Se evaluará la utilidad educativa mediante tres pruebas controladas:
1. **Prueba de Precisión (Test Técnico):** Comprobar si el resumen refleja los acuerdos reales y detecta alucinaciones.
2. **Revisión de Facilidad de Uso (Usabilidad):** Evaluar si la interfaz es agradable, clara y diferencia bien las categorías (Acuerdos, Tareas).
3. **Prueba de Utilidad Educativa:** Encuestar a los usuarios para saber si el sistema mejoró su comprensión de los objetivos y el trabajo en equipo.

### 🚀 Fase 6: Implementación y Seguimiento
Pondremos SICOCO a prueba en un curso real (Programa Piloto) por un tiempo definido. Se recopilará la opinión de los usuarios para mejorar el sistema y se contemplan futuras mejoras, como permitir elegir el estilo del resumen (Serio para informes, Rápido para reuniones de seguimiento).

---

## 🔮 Supuestos

- Se asume que los estudiantes saben exportar o trasladar chats desde sus plataformas de mensajería (ej. WhatsApp) al sistema.
- Se asume que los equipos mantienen una comunicación escrita lo suficientemente clara y estructurada para que una IA identifique intenciones de trabajo.
- Se cuenta con acceso a APIs de IA generativa bajo los planes gratuitos o en cuotas financiables por estudiantes.

---

## 🚧 Posibles Riesgos

- **Alucinación de la IA:** Que el modelo de lenguaje genere acuerdos o asigne tareas que el grupo nunca mencionó en realidad.
- **Resistencia al uso:** Que a los estudiantes les parezca tedioso el proceso de proveer el historial del chat al sistema.
- **Mala calidad de datos de entrada:** Que el chat esté lleno de audios, imágenes o stickers, limitando fuertemente el texto que la IA puede procesar.

---

## ❓ Preguntas Frecuentes (FAQ)

- **¿SICOCO funciona en tiempo real conectado a WhatsApp?**
  No. Por razones técnicas y de privacidad en este MVP, el historial deberá ser proveído al sistema de manera asíncrona.
- **¿Qué tipo de chats puede analizar?**
  Historiales generados por plataformas de comunicación colaborativa o transcripciones simples. El formato exacto (texto plano, u otros) dependerá de la arquitectura que se termine eligiendo.
- **¿Es seguro usarlo con tareas de la Universidad?**
  Sí, SICOCO procesará el texto sin almacenar datos sensibles por tiempo indefinido, enfocándose puramente en la extracción de aprendizaje.

---

## ✅ Criterios de Éxito

- La herramienta es capaz de leer un chat de al menos 100 mensajes y generar una síntesis funcional sin errores técnicos (timeouts).
- La precisión en la extracción de Tareas (qué hacer y quién debe hacerlo) resulta verídica frente a una revisión humana manual.
- El sistema se despliega en una interfaz accesible y cuenta con el feedback cualitativo positivo de los usuarios de prueba en la etapa de evaluación piloto.

---

## 🎤 Entrevista Técnica: Arquitectura de Datos de SICOCO

**Rol:** Arquitecto de Datos Senior  
**Objetivo:** Identificar los requerimientos para el modelado de la base de datos relacional del proyecto SICOCO, extrayendo las entidades, atributos y relaciones necesarias.

### 👥 Bloque 1: Usuarios, Roles y Organización Académica
**1. ¿Qué datos personales y académicos debemos registrar sobre cada estudiante que utilice SICOCO?**
> 💡 **Posible Respuesta (Datos):** Entidad `Estudiante` necesita almacenar: `ID_Estudiante` (Llave primaria), `Numero_Identidad_Matricula`, `Nombres`, `Apellidos`, `Correo_Institucional`, `Contraseña_Encriptada`, `Semestre_Actual`, `Programa_Academico` (Ej. Lic. en Informática), y `Fecha_Registro`.

**2. ¿Existen otros tipos de usuarios en el sistema además de los estudiantes, como profesores o administradores?**
> 💡 **Posible Respuesta (Datos):** Sí, necesitamos una entidad `Rol` o bien atributos extendidos para `Profesor`: `ID_Profesor`, `Numero_Empleado`, `Nombres`, `Apellidos`, `Departamento`, y nivel de `Permiso_Sistema`.

**3. ¿Cómo organizamos a los estudiantes académicamente dentro del sistema?**
> 💡 **Posible Respuesta (Datos):** A través de asignaturas o cursos. Entidad `Curso`: `ID_Curso`, `Codigo_Materia`, `Nombre_Materia` (Ej. Diseño de Software Educativo I), `Semestre_Academico` (Ej. 2026-1), y `ID_Profesor_Responsable`.

**4. Ya que SICOCO se basa en proyectos grupales, ¿cómo estructuramos los equipos de trabajo?**
> 💡 **Posible Respuesta (Datos):** Entidad `Equipo`: `ID_Equipo`, `Nombre_Equipo`, `ID_Curso` (asociado a qué curso pertenece), y `Fecha_Creacion`.

**5. ¿Cómo gestionamos a los integrantes de los equipos? ¿Un estudiante puede estar en varios equipos?**
> 💡 **Posible Respuesta (Datos):** Sí, se necesita una tabla intermedia `Miembro_Equipo`: `ID_Relacion`, `ID_Estudiante`, `ID_Equipo`, `Rol_En_Equipo` (Ej. Líder, Participante), y `Fecha_Union`.

### 💬 Bloque 2: Entradas de Datos (Chats y Sesiones de Trabajo)
**6. Cuando un equipo se reúne a discutir un proyecto, ¿qué datos guarda SICOCO de la propia reunión o sesión?**
> 💡 **Posible Respuesta (Datos):** Entidad `Sesion_Trabajo`: `ID_Sesion`, `ID_Equipo`, `Fecha_Reunion`, `Objetivo_General`, `Plataforma_Origen` (Ej. Discord, Teams, WhatsApp), y `Duracion_Estimada`.

**7. Los usuarios proveen el registro de su chat al sistema. ¿Qué información guardamos sobre este ingreso?**
> 💡 **Posible Respuesta (Datos):** Entidad `Registro_Chat`: `ID_Registro`, `ID_Sesion`, `Origen_Metadata` (URL, Path o Buffer), `Formato_Entrada` (txt, csv, JSON), `Tamaño_Datos`, y el `ID_Estudiante_Ingresa`.

**8. Antes del resumen, ¿es necesario guardar cada mensaje individual del chat en la base de datos por separado?**
> 💡 **Posible Respuesta (Datos):** Serviría mucho para precisión. Entidad `Mensaje_Original`: `ID_Mensaje`, `ID_Registro`, `Alias_Remitente`, `Cuerpo_Del_Mensaje` (Texto), `Fecha_Hora_Mensaje` (Timestamp).

### 🤖 Bloque 3: Procesamiento de IA (Ingeniería de Prompts y Motor)
**9. SICOCO utiliza distintos "tonos" o configuraciones para decirle a la IA cómo resumir. ¿Cómo guardamos estas instrucciones maestras (prompts)?**
> 💡 **Posible Respuesta (Datos):** Entidad `Configuracion_Prompt`: `ID_Configuracion`, `Nombre_Estilo` (Ej. Rápido, Serio/Formal), `Texto_Instruccion_IA`, y `Estado_Activo` (Booleano).

**10. ¿Qué detalles guardamos cuando el sistema finalmente produce un resumen del chat entero?**
> 💡 **Posible Respuesta (Datos):** Entidad `Resumen_Generado`: `ID_Resumen`, `ID_Sesion`, `Texto_Final_Plano` (por si la vista falla), `Modelo_IA_Usado` (Ej. Gemini-1.5, OpenAI), `Consumo_Tokens`, y `Fecha_Generacion`.

### 🏗️ Bloque 4: Pilares de Información (Los 4 Puntos Clave de Salida)
**11. Del punto pedagógico, sabemos que debemos capturar "Acuerdos". ¿Qué atributos componen un "Acuerdo"?**
> 💡 **Posible Respuesta (Datos):** Entidad `Acuerdo_Equipo`: `ID_Acuerdo`, `ID_Resumen`, `Descripcion_Solucion`, `Nivel_Importancia` (Alto/Medio/Bajo), y el/los `Alias_Quien_Propone`.

**12. También el resumen separa "Desacuerdos o Posturas Encontradas". ¿Qué datos nos pide esto?**
> 💡 **Posible Respuesta (Datos):** Entidad `Desacuerdo`: `ID_Desacuerdo`, `ID_Resumen`, `Tema_Debate`, `Descripcion_Oposicion`, y `Estado_Resolucion` (Resuelto / Activo).

**13. Para las "Dudas sin Resolver" que quedan al final de la reunión, ¿qué debemos registrar?**
> 💡 **Posible Respuesta (Datos):** Entidad `Duda_Abierta`: `ID_Duda`, `ID_Resumen`, `Pregunta_Principal`, `Relacionado_Con_Tema` (Ej. Base de datos, Interfaz).

**14. SICOCO crea un "To-Do" (Tareas a hacer). ¿Cuáles son las columnas indispensables para la base de datos de las Tareas?**
> 💡 **Posible Respuesta (Datos):** Entidad `Tarea_Asignada`: `ID_Tarea`, `ID_Resumen`, `Titulo_Actividad`, `ID_Estudiante_Asignado` (FK al estudiante), `Estatus` (Pendiente, En Proceso, Hecha), y `Fecha_Limite` o sugerida.

### 🗺️ Bloque 5: Mapeo de Co-Creación (Línea de Tiempo)
**15. Mencionaste mostrar cómo evolucionan las ideas con una "Línea de tiempo". ¿Cómo guardaremos esta cronología de forma estructurada?**
> 💡 **Posible Respuesta (Datos):** Entidad `Momento_Clave_Chat`: `ID_Momento`, `ID_Resumen`, `Marca_Tiempo_Aproximada`, `ID_Mensaje_Relacionado`, `Alias_Usuario`, y `Evento` ("Idea Nueva", "Solución", "Pregunta").

**16. ¿La base de datos buscará relacionar u enlazar quién aportó a la solución final de qué otra persona?**
> 💡 **Posible Respuesta (Datos):** Puede requerir una Tabla de Relación Recursiva o intermedia `Conexion_Idea`: `ID_Idea_Base`, `ID_Aporte_Extra`, para dibujar cómo las ideas se alimentan mutuamente en la vista.

### 📈 Bloque 6: Evaluación y Pruebas (Feedback de la Herramienta)
**17. Si hacemos una prueba técnica al resumen (Fase 5), ¿qué información se audita sobre la calidad del resumen?**
> 💡 **Posible Respuesta (Datos):** Entidad `Control_Calidad_Bot`: `ID_Test`, `ID_Resumen`, `Cantidad_Falsos_Positivos`, `Calificacion_Fidelidad_texto` (Del 1 al 10), y `Comentario_Técnico`.

**18. En la "Prueba de Facilidad de Uso", recogeremos datos de experiencia del usuario (UX). ¿Qué se guardará aquí?**
> 💡 **Posible Respuesta (Datos):** Entidad `Evaluacion_UX`: `ID_Eval_UX`, `ID_Estudiante`, `Claridad_Visual` (1-5), `Separacion_Vista_Tareas` (Booleano: ¿Fue claro?), y `Sugerencias_Extra` (Texto grande).

**19. Queremos medir el impacto educativo en los estudiantes (si sienten que mejoró su trabajo). ¿Qué atributos forman esa encuesta de "Utilidad"?**
> 💡 **Posible Respuesta (Datos):** Entidad `Encuesta_Piloto`: `ID_Encuesta`, `ID_Estudiante`, `Mejor_Comprension_Objetivos_Si_No` (Booleano), `Nivel_de_Apoyo_En_Grupo` (Escala Likert 1 al 5), y `Fecha_Respuesta`.

### 🔒 Bloque 7: Escalabilidad, Privacidad y Seguridad
**20. Como SICOCO alberga los chats de personas y puede escalar a un entorno universitario permanente, ¿qué campos de infraestructura y permisos tenemos para asegurar su privacidad?**
> 💡 **Posible Respuesta (Datos):** Cada tabla requerirá campos de `Created_At` (Fecha creación) y `Updated_At`. El registro del chat tendrá una bandera `Es_Confidencial` y los equipos de trabajo `Requiere_Aprobacion_Profesor`. Los IDs deben ser encriptados o en formato UUID para evitar fuga o que otros equipos miren los acuerdos de la competencia.

---

## 📖 Matriz de Historias de Usuario - Proyecto SICOCO

**Basado en Arquitectura de Datos y Metodología MODESEC**

### 🧑‍🤝‍🧑 ZONA 1: Usuarios, Roles y Organización (PER)
**Entidades:** Estudiante, Profesor, Administrador, Curso y Equipo.

| ID | Historia (Como / Quiero / Para) | Valor | Prioridad | Dependencias | Criterios de aceptación |
| :--- | :--- | :---: | :---: | :---: | :--- |
| **PER-01** | Como estudiante, quiero registrarme con mi ID, programa y semestre para ser identificado en el sistema. | Alta | Must | Ninguna | Dado que ingreso mis datos académicos.<br>Cuando guardo<br>Entonces se crea el registro en la entidad Estudiante. |
| **PER-02** | Como docente, quiero vincularme a una asignatura para supervisar los grupos de trabajo. | Alta | Must | PER-01 | Dado que el usuario tiene rol Docente.<br>Cuando selecciona una asignatura<br>Entonces queda asignado como mentor del curso. |
| **PER-03** | Como estudiante, quiero poder actualizar mi contraseña desde mi perfil para mantener mi cuenta segura sin depender de envíos de correo. | Media | Should | PER-01 | Dado que estoy logueado.<br>Cuando voy a mi perfil y edito la clave<br>Entonces se actualiza en la base de datos localmente. |
| **PER-04** | Como integrante de equipo, quiero ser vinculado a un ID_Equipo para trabajar colaborativamente. | Alta | Must | PER-01 | Dado un grupo creado.<br>Cuando el admin me añade<br>Entonces mi ID se relaciona con el ID_Equipo. |

### 📂 ZONA 2: Entradas y Sesiones de Trabajo (SES)
**Manejo de la entidad:** Reunión, Registro_Chat y Mensajes individuales.

| ID | Historia (Como / Quiero / Para) | Valor | Prioridad | Dependencias | Criterios de aceptación |
| :--- | :--- | :---: | :---: | :---: | :--- |
| **SES-01** | Como estudiante, quiero crear una Sesión de Trabajo con fecha y hora para iniciar la co-creación. | Alta | Must | PER-04 | Dado un ID_Equipo.<br>Cuando se abre la sesión<br>Entonces se genera el registro en la entidad Sesion_Trabajo. |
| **SES-02** | Como estudiante, quiero ingresar el historial de chat para que el sistema administre el registro físico/digital. | Alta | Must | SES-01 | Dado un registro de chat.<br>Cuando se ingresa<br>Entonces se guarda la ruta, origen o metadata en la tabla Registro. |
| **SES-03** | Como sistema, quiero separar los mensajes individuales (Cuerpo y Autor) para analizarlos por separado. | Alta | Must | SES-02 | Dado un registro ingresado.<br>Cuando se procesa<br>Entonces cada línea se guarda con su ID_Autor y Marca_Tiempo. |
| **SES-04** | Como usuario, quiero ver el historial de registros ingresados por sesión para evitar duplicar información. | Media | Should | SES-02 | Dado una sesión activa.<br>Cuando consulto registros<br>Entonces el sistema lista las fechas y orígenes de carga. |

### 🤖 ZONA 3: Motor de IA y Procesamiento (IA)
**Uso de:** Ingeniería de Prompts y categorización (Acuerdos, Tareas, Dudas).

| ID | Historia (Como / Quiero / Para) | Valor | Prioridad | Dependencias | Criterios de aceptación |
| :--- | :--- | :---: | :---: | :---: | :--- |
| **IA-01** | Como sistema, quiero categorizar mensajes en Acuerdos, Dudas y Tareas para estructurar la síntesis. | Alta | Must | SES-03 | Dado el texto del chat.<br>Cuando la IA procesa<br>Entonces asigna una categoría a cada punto clave. |
| **IA-02** | Como sistema, quiero extraer tareas (To-Do) con descripción y responsable para organizar el trabajo. | Alta | Must | IA-01 | Dado un compromiso detectado.<br>Cuando la IA lo procesa<br>Entonces se crea una fila en la tabla Tarea con su Responsable. |
| **IA-03** | Como estudiante, quiero que la IA identifique dudas sin resolver para que el grupo las retome luego. | Media | Should | IA-01 | Dado una pregunta sin respuesta en el chat.<br>Cuando termina el análisis<br>Entonces se lista en Dudas_Pendientes. |
| **IA-04** | Como sistema, quiero identificar los temas más repetidos (palabras clave) para que el grupo sepa en qué se enfocaron más. | Baja | Could | IA-01 | Dado el texto del chat.<br>Cuando la IA procesa<br>Entonces genera una lista simple de los temas más frecuentes. |

### 📊 ZONA 4: Visualización y Línea de Tiempo (GUI)
**Entidades:** Mapeo de Co-creación y visualización de hitos.

| ID | Historia (Como / Quiero / Para) | Valor | Prioridad | Dependencias | Criterios de aceptación |
| :--- | :--- | :---: | :---: | :---: | :--- |
| **GUI-01** | Como estudiante, quiero ver una línea de tiempo con los hitos del chat para entender la evolución de las ideas. | Alta | Should | IA-01 | Dado el resumen generado.<br>Cuando cargo la vista<br>Entonces se muestran los elementos de la tabla Hito_Cronologico. |
| **GUI-02** | Como usuario, quiero ver el nombre del autor original junto a cada acuerdo o idea para reconocer quién lo propuso. | Media | Should | GUI-01 | Dado un resumen generado.<br>Cuando leo los acuerdos<br>Entonces veo el alias del autor al lado en texto plano. |
| **GUI-03** | Como estudiante, quiero elegir entre un estilo de resumen Serio o Rápido según mi necesidad. | Media | Could | IA-04 | Dado el resumen finalizado.<br>Cuando selecciono estilo<br>Entonces la visualización cambia el nivel de detalle. |
| **GUI-04** | Como estudiante, quiero ver el resumen dividido por categorías para leer solo lo que me interesa. | Alta | Must | IA-01 | Dado el resumen generado.<br>Cuando se carga el dashboard<br>Entonces aparecen pestañas por cada categoría. |

### 🛡️ ZONA 5: Evaluación y Seguridad (EVA)
**Control de Calidad:** Auditoría y Privacidad (Created_At, Updated_At).

| ID | Historia (Como / Quiero / Para) | Valor | Prioridad | Dependencias | Criterios de aceptación |
| :--- | :--- | :---: | :---: | :---: | :--- |
| **EVA-01** | Como docente, quiero calificar la fidelidad del resumen (1-10) para evaluar el desempeño técnico. | Media | Should | GUI-01 | Dado un resumen revisado.<br>Cuando el docente califica<br>Entonces se guarda en Control_Calidad_IA. |
| **EVA-02** | Como estudiante, quiero poder editar manualmente el resumen generado por la IA para corregir pequeños errores antes de guardarlo. | Alta | Must | GUI-01 | Dado un resumen en pantalla.<br>Cuando presiono "Editar"<br>Entonces se abre un campo de texto para corregirlo y guardarlo. |
| **EVA-03** | Como administrador, quiero un historial de modificaciones para auditar quién cambió un resumen. | Alta | Must | GUI-01 | Dado un cambio en los datos.<br>Cuando se guarda<br>Entonces se actualiza el campo Updated_At y el ID_Editor. |
| **EVA-04** | Como sistema, quiero restringir el acceso a usuarios no autorizados para proteger la privacidad del grupo. | Alta | Must | PER-04 | Dado un intento de consulta anónima.<br>Cuando se valida el rol<br>Entonces el sistema bloquea la vista si no pertenece al equipo. |
