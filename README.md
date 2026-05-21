# Talleres de Aprendizaje Profundo

Talleres 1 a 4 del curso de Aprendizaje Profundo de la Maestría en Ciencia de
Datos y Analítica. Cada taller aborda una familia de arquitecturas de redes
neuronales, desde redes densas hasta modelos basados en *Transformers*.

## Estructura

| Carpeta | Tema |
|---|---|
| `Taller1-DNN` | Redes densas (MLP) |
| `Taller2-CNN` | Redes convolucionales |
| `Taller3-RNN` | Redes recurrentes |
| `Taller4-Transformers` | Transformers y *fine-tuning* |

## Talleres

### Taller 1 — DNN
Red neuronal multicapa (MLP) para clasificación de imágenes sobre el dataset
Intel Image Classification.
- `si7011-mlp-intel.ipynb` — notebook ejecutado.
- `predictions.csv` — predicciones generadas.

### Taller 2 — CNN
Red neuronal convolucional para clasificación de imágenes sobre Tiny ImageNet.
- `si7011-cnn-tinyimagenet.ipynb` — notebook ejecutado.
- `best_cnn.pt` — pesos del mejor modelo.
- `submission.csv` — predicciones generadas.

### Taller 3 — RNN
Red neuronal recurrente (GRU) para predicción sobre series de tiempo.
- `part-1-data.ipynb` — preparación y exploración de los datos.
- `part-2-model.ipynb` — definición, entrenamiento y evaluación del modelo.
- `best_model.pt` — pesos del mejor modelo.
- `data/bike_processed/` — datos preprocesados.
- `runs/` — registros de TensorBoard del entrenamiento.

### Taller 4 — Transformers
Clasificación de texto sobre el benchmark TweetEval, desarrollada en seis partes:
- `tweeteval-part-1-data.ipynb` — preparación de los datos.
- `tweeteval-part-2-pipeline.ipynb` — pipeline de procesamiento y evaluación.
- `tweeteval-part-3-distilbert.ipynb` — *fine-tuning* de DistilBERT.
- `tweeteval-part-4-bertweet.ipynb` — *fine-tuning* de BERTweet.
- `tweeteval-part-5-lora.ipynb` — ajuste fino eficiente con LoRA.
- `tweeteval-part-6-deployment.ipynb` — despliegue del modelo.

## Tecnologías

- Python
- PyTorch
- Hugging Face (`transformers`, `datasets`, `peft`)
- scikit-learn

## Uso

Los notebooks se entregan **ya ejecutados, con sus salidas visibles**, por lo
que pueden revisarse sin necesidad de correrlos.

Fueron desarrollados sobre **Kaggle** (Talleres 1–3) y **LightningAI**
(despliegue del Taller 4): entornos con las dependencias preinstaladas y acceso
a los datasets. Reproducirlos requiere ese entorno — las dependencias no se
declaran en este repositorio, los Talleres 1 y 2 usan rutas de datos propias de
Kaggle, y entrenar los modelos de Transformers requiere GPU.

## Autor

Elkin Ortiz R. — edortizr@eafit.edu.co
