# Overview: Image Sharpening using Knowledge Distillation

A lightweight student model is trained to sharpen blurred images by learning from a heavy teacher model (Restormer). Two students are trained independently on separate datasets (mine and my friend's), and their outputs are combined using an ensemble strategy.

##  Features

-  Uses **Restormer** as the teacher model.
-  Two student models trained separately on different datasets.
-  Ensemble inference combining student predictions.
-  Lightweight, fast, and effective for real-time sharpening.

##  How It Works

1. **Restormer** generates sharp targets for blurred inputs.
2. **Student A** and **Student B** are trained using knowledge distillation(L1 loss and Perceptual loss functions).
3. At test time, outputs of both students are **combined (ensemble)** to produce the final image

##  Evaluation Metrics

- SSIM (Structural Similarity)

##  Contributors

- **Aditya Toley** — Training Student A, ensemble logic, evaluation
- **Nikhil Narayanan O** — Training Student B, dataset management
