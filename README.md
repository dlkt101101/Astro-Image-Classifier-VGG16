# Astrophysical Body Image Classifier: Benchmarking CNN Architectures on Deep-Sky Imagery

![Classification examples](docs/images/astro_grid.png)
*Sample predictions across 12 astrophysical classes — galaxies, nebulae, star clusters*

## The Problem
Astronomical surveys generate millions of images faster than they can be
manually labeled. Our team (3 members) tackled a 12-class astrophysical
object classification problem, each of us independently building and
tuning a different CNN architecture to compare approaches on the same
dataset — a mini bake-off to find what actually works for this domain.

**My role:** Implemented and fine-tuned VGG16, including transfer-learning
setup, augmentation strategy, and hyperparameter tuning (`VGG16_Darren.ipynb`).

## Results

| Model | Owner | Test Accuracy | F1 (macro) |
|---|---|---|---|
| VGG16 (fine-tuned) | Darren | [X]% | [X] |
| ResNet50 | Raghuv | [X]% | [X] |
| Custom CNN | Ojus | [X]% | [X] |

![Confusion matrix](docs/images/confusion_matrix.png)
*Confusion matrix, VGG16 — most confusion occurs between [class A] and [class B],
likely due to [visual similarity reason]*

![Grad-CAM saliency](docs/images/gradcam_examples.png)
*Grad-CAM overlays showing the model attends to [nucleus/spiral arms/etc.]
when classifying [class]*

## Dataset
12-class astrophysical object dataset ([Kaggle link](https://www.kaggle.com/datasets/engeddy/astrophysical-objects-image-dataset/data)).
Not included in this repo due to size — see notebooks for download instructions.

## Full Writeup
See [Project Report.pdf](./Project%20Report.pdf) for the complete methodology,
per-model comparison, and error analysis.

## Repo Structure
```
├── VGG16_Darren.ipynb        # my model implementation
├── ResNet50_Raghuv.ipynb
├── CustomCNN_Ojus.ipynb
└── Project Report.pdf
```
