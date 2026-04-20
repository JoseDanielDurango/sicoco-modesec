# 💻 Fase 3: Diseño Computacional (Arquitectura Técnica)

Este es el plan básico para desarrollar el programa bajo un modelo **MVP (Producto Mínimo Viable)**. Esto asegura que el proyecto mantenga un alcance realista y se pueda culminar satisfactoriamente durante el semestre universitario.

---

## 📥 Entrada de Datos (Básica y Segura)

Para evitar la complejidad técnica de integraciones con APIs externas o web scraping en vivo (ej. bots en Discord o Telegram), el sistema recibirá la información de manera unificada:

- 🟢 **Ingreso de Historiales (Sujeto a Evaluación):** Se proveerá una interfaz sencilla (ya sea una aplicación web, un programa de escritorio local, o una extensión de navegador, aún por definir) donde el estudiante ingresará el historial exportado de sus chats de trabajo grupal.

> ⚠️ *(Nota: Esta restricción asegura la factibilidad del proyecto para el equipo de desarrollo, eludiendo problemas de tokens en tiempo real, bloqueos de plataformas y políticas de privacidad en tiempo real).*

---

## ⚙️ El Motor de SICOCO (Procesamiento)

SICOCO funcionará consumiendo las APIs de Inteligencias Artificiales generativas comerciales de bajo costo o capa gratuita (como Gemini o OpenAI). 

- 🤖 **Enfoque en Ingeniería de Prompts:** No se entrenará una IA desde cero (fine-tuning). Se utilizará un sistema robusto de instrucciones estructuradas.
- 📜 La instrucción matriz dirigirá al modelo de lenguaje para que extraiga precisamente nuestros cuatro ejes metacognitivos: **acuerdos, tareas, desacuerdos y dudas.**

---

## 🖥️ Pantalla para el Usuario (UI)

Se construirá una interfaz gráfica (Dashboard) estructurada y clara, sin requerir elementos dinámicos excesivamente complejos. 

> 💡 Lo primordial es exponer de manera visual los elementos extraídos, como identificar al autor del acuerdo y enlistar las tareas pendientes, para que cualquier miembro del equipo comprenda el estatus general de un solo vistazo.
