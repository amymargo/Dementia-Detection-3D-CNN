# Dementia Detection Using 3D CNNs

This project applies deep learning to MRI neuroimaging data to classify dementia vs. non-dementia cases using a custom 3D Convolutional Neural Network. The work includes extensive preprocessing (registration, skull stripping, noise correction) and a ResNet-inspired model architecture designed for high-dimensional medical imaging.

Authors: Amy Margolina, Michael Batushansky, and Alexander Hajdukiewicz

---

## Files

### 1. `Dementia_Detection.ipynb`

This is the main notebook and includes:

- Dataset loading  
- Preprocessing steps (registration, skull stripping, N4 bias correction)  
- Conversion to HDF5 format  
- 3D CNN model architecture  
- Training, validation, and testing workflow  
- Performance metrics (accuracy, F1 score, recall, precision)  
- Loss and evaluation plots  

Run this notebook in **Google Colab** with GPU acceleration enabled.

---

### 2. `Project_Report.pdf`

A full written report containing:

- Medical and scientific motivation  
- Dataset description and limitations  
- Detailed preprocessing pipeline  
- Model architecture and hyperparameters  
- Evaluation metrics and analysis  
- Challenges and recommendations for future work  

---

### 3. `Deep_Learning_Presentation.pdf`

A slide presentation summarizing:

- Project overview  
- Dataset and preprocessing  
- Model design  
- Training results  
- Key insights  

---

## Dataset

This project uses the **OASIS-2 MRI dataset** (T1-weighted structural scans).  
The dataset **cannot be uploaded to GitHub** due to licensing restrictions.

To access the data, request it from:  
https://sites.wustl.edu/oasisbrains/home/oasis-2/

Once downloaded, update the paths in the notebook before running.

---

## How to Run the Notebook

1. Open `Dementia_Detection.ipynb` in Google Colab  
2. Go to **Runtime → Change runtime type → GPU**  
3. Upload or mount your dataset  
4. Run the notebook from top to bottom  

Training may require a GPU with high memory.  
For smaller GPUs, reduce batch size or image dimensions.

---

## Model Performance Summary

After preprocessing (N4 bias correction + improved skull stripping), the model achieved:

- **Accuracy:** ~73%  
- **F1 Score:** ~70%  
- **Recall (Dementia class):** ~92%  
- **Precision (Non-Dementia class):** ~82%  

Preprocessing improved performance significantly compared to raw images.
