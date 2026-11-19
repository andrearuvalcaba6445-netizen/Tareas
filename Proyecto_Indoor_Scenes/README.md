# Proyecto: Clasificación y Aumento Sintético en Indoor Scenes

Este repositorio contiene las prácticas de Deep Learning aplicadas al reconocimiento de escenas interiores (*Indoor Scenes*).

## Contenido del Repositorio

* **`Indoor_scenes_U3_Teoria_Transfer_Learning__corregido.ipynb`**: Implementación y evaluación de modelos mediante Transfer Learning sobre el conjunto de datos de escenas interiores.
* **`U3_S6_Practica_cGAN_FID_Aumento_Sintetico_DL.ipynb`**: Entrenamiento de una Red Generativa Antagónica Condicional (cGAN), evaluación de calidad mediante FID y exactitud condicional, y comparación entre aumento de datos clásico y generación sintética aplicada al dataset de escenas interiores.

## Conjunto de Datos (Dataset)

Debido al tamaño del conjunto de datos (~2.5 GB), los archivos de imagen no se almacenan directamente en este repositorio. Ambos cuadernos descargan el dataset de forma automática desde Hugging Face mediante la librería `datasets`:

* **Nombre en Hugging Face:** [`FatimaSaadNaik/indoor-scenes-dataset`](https://huggingface.co/datasets/FatimaSaadNaik/indoor-scenes-dataset)
* **Total de registros:** 15,620 imágenes etiquetadas por categoría de escena interior.

### Código de carga utilizado
```python
from datasets import load_dataset
ds = load_dataset("FatimaSaadNaik/indoor-scenes-dataset")
