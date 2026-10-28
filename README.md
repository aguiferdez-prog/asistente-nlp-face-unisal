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

1. Abre el notebook en Google Colab.
2. Sube al entorno de Colab la base de conocimiento (`.xlsx`).
3. Ejecuta las celdas en orden.

## Autora

Janina Aguilera.
