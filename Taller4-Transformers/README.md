# Taller 4 — Transformers

Clasificación de emociones sobre el benchmark TweetEval mediante *fine-tuning*
de modelos basados en Transformers.

## Modelos entrenados

Los modelos entrenados están publicados en Hugging Face Hub. No se incluyen en
este repositorio por su tamaño; cada uno corresponde a un notebook:

| Modelo | Notebook | Enlace |
|---|---|---|
| DistilBERT | `tweeteval-part-3-distilbert.ipynb` | https://huggingface.co/ElOrtiz/tweeteval-emotion-distilbert |
| BERTweet | `tweeteval-part-4-bertweet.ipynb` | https://huggingface.co/ElOrtiz/tweeteval-emotion-bertweet |
| BERTweet + LoRA (merged) | `tweeteval-part-5-lora.ipynb` | https://huggingface.co/ElOrtiz/tweeteval-emotion-bertweet-lora |

## Cargar un modelo

```python
from transformers import pipeline

clf = pipeline("text-classification",
               model="ElOrtiz/tweeteval-emotion-bertweet",
               top_k=None)
clf("I'm so happy today!")
```
