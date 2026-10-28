# Asistente virtual con NLP para consultas institucionales (FACE-UNISAL)

Proyecto del Diplomado en Inteligencia Artificial Aplicada (Instituto Desarrollo, 2026).

## Descripción

Prototipo de asistente virtual que clasifica consultas de estudiantes sobre trámites e información de la Facultad (FACE-UNISAL) y responde a partir de una base de conocimiento validada. Cuando una consulta requiere atención de una persona, el asistente no responde de forma automática y la deriva a atención humana.

## Qué incluye

- Dataset etiquetado de 220 consultas institucionales en 7 categorías.
- Comparación de 4 modelos de clasificación: Naive Bayes, Regresión Logística, red neuronal y un modelo base de referencia.
- Prototipo funcional con umbrales de confianza y una regla estricta de derivación a atención humana.
- Base de conocimiento de 9 hojas, con vacíos de información resueltos mediante confirmaciones de la Secretaría Académica.

## Contenido del repositorio

| Archivo | Descripción |
|---|---|
| `Notebook_Final_Consolidado` | Código del proyecto: preparación de datos, entrenamiento, comparación de modelos y prototipo. |
| `Base_Conocimiento_FACE-UNISAL.xlsx` | Base de conocimiento con las categorías, consultas y respuestas validadas. |
| `Protocolo_Derivacion_Humana.pdf` | Protocolo que define cuándo una consulta debe derivarse a una persona. |

## Cómo funciona

1. El usuario escribe una consulta.
2. El modelo la clasifica en una de las categorías.
3. Si la confianza de la predicción supera el umbral y la categoría no requiere atención humana, el asistente responde con la información de la base de conocimiento.
4. Si la confianza es baja o la consulta pertenece a una categoría que debe derivarse, el asistente indica que la atenderá una persona.

## Tecnologías

Python, Pandas, Scikit-learn, Matplotlib y Google Colab.

## Cómo ejecutarlo

No necesitas instalar nada. Solo necesitas una cuenta de Google.

1. Descarga el archivo del notebook desde este repositorio.
2. Entra a [Google Colab](https://colab.research.google.com) y sube el notebook (Archivo → Subir cuaderno).
3. En el menú superior elige **Entorno de ejecución → Ejecutar todo** y espera a que terminen todas las celdas.
4. Baja hasta el final, a la sección **7. Prototipo funcional consolidado**, y usa la **interfaz de demostración tipo chat** (opcional, pensada para presentaciones).
5. Escribe una consulta en el chat, por ejemplo: *"¿Cuantas horas de extensión por año necesito?"*, y el asistente responderá o la derivará a una persona.

> **Importante:** debes ejecutar todo el notebook antes de probar el chat; si no, la interfaz no funcionará.

## Autora

Janina Aguilera.
