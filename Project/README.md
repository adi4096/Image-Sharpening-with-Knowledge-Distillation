# Project Folder Structure – Breakdown

This document explains the internal folder structure of the "Image Sharpening using Knowledge Distillation" project. 
This file focuses on describing the contents of each subdirectory.

---

## Dataset/

Contains dataset-related resources.

- `Script for preparing dataset`  
  Python script used to prepare the dataset, including splitting into training, testing, and showcase sets.

---

## Notebooks/

Contains all Jupyter notebooks used for training, evaluation, and ensemble inference.

- `ProjectRun_SetA.ipynb`  
  Trains and evaluates the student model using Dataset A.

- `ProjectRun_SetB.ipynb`  
  Trains and evaluates the student model using Dataset B.

- `BothWeights.ipynb`  
  Performs ensemble inference by combining outputs of both student models.

---

## Restomer/

Includes files related to the teacher model (Restormer).

- `Readme.md`  
  Documents the source of the Restormer architecture and pretrained weights:
  - Architecture: [restormer_arch.py](https://raw.githubusercontent.com/swz30/Restormer/main/basicsr/models/archs/restormer_arch.py)
  - Weights: [Google Drive Folder](https://drive.google.com/drive/folders/1bRBG8DG_72AGA6-eRePvChlT5ZO4cwJ4)

---

## Weights/

Holds the trained weights of the student models.

- `Train_A.pth`  
  Student model weights trained on Dataset A.

- `Train_B.pth`  
  Student model weights trained on Dataset B.

