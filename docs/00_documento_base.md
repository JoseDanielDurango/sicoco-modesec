# 📖 Documento Base de SICOCO

**Contexto Académico:**
El proyecto **SICOCO (Sintetizador de Co-creación Colaborativa)** nace como una iniciativa de los estudiantes de **8vo semestre** de la **Licenciatura en Informática con énfasis en medios audiovisuales** de la **Universidad de Córdoba**. Desarrollado bajo la materia de **Diseño y Desarrollo de Software Educativo I**, empleando la metodología pedagógica **MODESEC**.

---

## 📝 Descripción del Proyecto

SICOCO es una herramienta digital de procesamiento de texto basada en Inteligencia Artificial diseñada para analizar, clasificar y resumir transcripciones de chats y foros de trabajo grupal. Su propósito no es solo resumir información, sino servir como una guía de apoyo que le permita a los estudiantes visualizar cómo colaboran, fomentando el trabajo en equipo.

---

## ⚠️ El Problema

El entorno de aprendizaje actual exige que los estudiantes trabajen en equipo utilizando herramientas asíncronas y chats de mensajería (WhatsApp, Discord, Teams). Esto genera una **sobrecarga de información**, provocando que valiosas ideas, debates importantes y acuerdos consensuados se pierdan o se olviden en medio de extensas cadenas de mensajes.

---

## 💡 La Solución Propuesta

Desarrollar un Producto Mínimo Viable (cuyo formato de despliegue está sujeto a evaluación técnica y podría ser una app web, un programa local, una extensión, etc.) que permita a los estudiantes ingresar sus historiales de chat grupal y utilizar Inteligencia Artificial para extraer de forma estructurada los puntos más importantes de la discusión, categorizándolos visualmente.

---

## 👥 Usuarios Objetivo

- **🎓 Estudiantes Universitarios y Escolares:** Principales beneficiarios que buscan optimizar su tiempo y no perder el hilo de sus proyectos grupales.
- **👨‍🏫 Docentes:** Que requieren observar o validar el verdadero nivel de participación, los debates y los consensos a los que llegan los grupos de estudiantes fuera del aula.

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

## 🔮 Supuestos

- Se asume que los estudiantes saben exportar o trasladar chats desde sus plataformas de mensajería (ej. WhatsApp) al sistema, independientemente de si finalmente se requiere una carga de archivo o copiar texto directamente.
- Se asume que los equipos mantienen una comunicación escrita lo suficientemente clara y estructurada para que una IA identifique intenciones de trabajo.
- Se cuenta con acceso a APIs de IA generativa (OpenAI, Gemini o similares) bajo los planes gratuitos o en cuotas financiables por estudiantes.

---

## 🚧 Posibles Riesgos

- **Alucinación de la IA:** Que el modelo de lenguaje genere acuerdos o asigne tareas que el grupo nunca mencionó en realidad.
- **Resistencia al uso:** Que a los estudiantes les parezca tedioso el proceso de proveer el historial del chat al sistema (por ejemplo, si el formato final exige descargas manuales muy largas).
- **Mala calidad de datos de entrada:** Que el chat esté lleno de audios, imágenes o stickers, limitando fuertemente el texto que la IA puede procesar y afectando el resumen final.

---

## ❓ Preguntas Frecuentes (FAQ)

- **¿SICOCO funciona en tiempo real conectado a WhatsApp?**
  No. Por razones técnicas y de privacidad en este MVP, el historial deberá ser proveído al sistema de manera asíncrona. El método exacto de ingreso (carga de archivo, copy/paste, extensión) aún se encuentra en etapa de diseño y evaluación.
- **¿Qué tipo de chats puede analizar?**
  Historiales generados por plataformas de comunicación colaborativa o transcripciones simples. El formato exacto (texto plano, u otros) dependerá de la arquitectura que se termine eligiendo.
- **¿Es seguro usarlo con tareas de la Universidad?**
  Sí, SICOCO procesará el texto sin almacenar datos sensibles por tiempo indefinido, enfocándose puramente en la extracción de aprendizaje.

---

## ✅ Criterios de Éxito

- La herramienta es capaz de leer un chat de al menos 100 mensajes y generar una síntesis funcional sin errores técnicos (timeouts).
- La precisión en la extracción de Tareas (qué hacer y quién debe hacerlo) resulta verídica frente a una revisión humana manual.
- El sistema se despliega en una interfaz accesible y cuenta con el feedback cualitativo positivo de los usuarios de prueba en la etapa de evaluación piloto.

