# Modelo de Lenguaje a Nivel de Carácter

Este proyecto implementa modelos de lenguaje basados en redes neuronales recurrentes (RNN, LSTM, GRU) para generar texto en español a nivel de carácter. Utiliza un corpus de literatura clásica española del Proyecto Gutenberg.

## Características

- **Modelos implementados**: SimpleRNN, LSTM y GRU (versiones básicas y avanzadas con capas apiladas).
- **Estrategias de generación**: Greedy Search, Beam Search y Sampling con temperatura.
- **Métricas de evaluación**: Pérdida, precisión, perplejidad y análisis lingüístico con SpaCy.
- **Dataset**: Corpus de ~7.5M caracteres de 8 libros clásicos españoles.

## Instalación

1. Clona el repositorio:
   ```bash
   git clone https://github.com/RodrigoGoni/chatbot.git
   cd chatbot
   ```

2. Instala las dependencias:
   ```bash
   pip install -r requirement.txt
   ```

3. Descarga el modelo de SpaCy (opcional para análisis):
   ```bash
   python -m spacy download es_core_news_sm
   ```

## Uso

Ejecuta el notebook `desafio3.ipynb` en Jupyter para:
- Entrenar los modelos (si no existen).
- Generar texto con diferentes semillas y estrategias.
- Visualizar métricas de entrenamiento.
- Analizar calidad del texto generado.

Los modelos entrenados y el dataset están almacenados en Git LFS.

## Archivos principales

- `desafio3.ipynb`: Notebook principal con todo el código.
- `corpus_espanol.txt`: Dataset de texto (Git LFS).
- `model_*.keras`: Modelos entrenados (Git LFS).
- `training_summary.csv`: Resumen de métricas.

## Resultados

- **Mejor modelo**: LSTM (val_perplexity: 3.51, val_accuracy: 0.60).
- Los modelos generan texto coherente, con LSTM mostrando mejor estructura gramatical.

Para más detalles, revisa el notebook y el informe incluido.