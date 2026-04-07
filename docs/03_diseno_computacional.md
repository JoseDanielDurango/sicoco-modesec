# Fase 3: Diseño Computacional (Cómo está hecho)

Este es el plan básico para hacer el programa bajo un modelo **MVP (Producto Mínimo Viable)**. Esto asegura que el proyecto no sea demasiado grande y se pueda terminar en un semestre de la universidad.

## Entrada de Datos (Básica y Segura)

Para evitar que el proyecto se vuelva demasiado difícil, el sistema recibirá la información de dos maneras:
- **Opción A (Recomendada):** Una pantalla web sencilla donde la persona sube manualmente un archivo (`.txt` o `.csv`) con los mensajes copiados de sus chats de trabajo.
- **Opción B (Alternativa):** Un bot sencillo que solo funcione en un programa (como Discord) para guardar los mensajes de un canal.

*(Nota: Por ahora, es mejor no conectar programas en vivo como Zoom, Slack y Telegram al mismo tiempo. Así nos aseguramos de poder entregar el proyecto y nos centramos en la parte educativa).*

## El Motor de SICOCO (Procesamiento)

SICOCO funcionará usando las inteligencias artificiales creadoras de texto que ya existen (como OpenAI, Gemini, Claude). 
- **No vamos a crear una IA desde cero.** En lugar de eso, usaremos un sistema basado en darle buenas instrucciones a la IA (Ingeniería de Prompts).
- La instrucción principal le dirá a la IA que lea el texto y busque nuestras cuatro partes clave: acuerdos, tareas, desacuerdos y dudas.

## Pantalla para el Usuario (UI)

Haremos una pantalla de resumen sencilla y clara. Mostraremos la información de forma fácil de entender, sin usar gráficos complicados. 
Lo más importante es mostrar las cuatro partes de la Fase 2 de manera muy visual. Así, cualquier estudiante que no haya estado en la reunión podrá entender lo que pasó de un solo vistazo.
