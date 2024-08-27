# Short Tracts Automatic Segmentation

Welcome to the Short Tracts Automatic Segmentation repository. This repository contains the necessary code, weights, and data for automating the segmentation of short tracts, including anterior, posterior, and hippocampal commissures, fornix, and uncinate fasciculus.

## Data
This repository consists of two datasets: the public dataset and the local hospital dataset. Each dataset includes training (n=100), validation (n=15), and test (n=60) images, containing peak images (input) and corresponding binary masks (output/ground truth). All data is anonymized, but you can find informations such as age and sex in the excel file. 

The binary masks cover 11 different tracts, comprising 5 short tracts: Anterior Commissure (AC), Posterior Commissure (PC), Hippocampal Commissure (HC), left and right Fornix (FX), and left and right Uncinate Fasciculus (UF). Additionally, there are 2 long tracts: Cortical Spinal Tract (CST) and Inferior Front-Occipital Fasciculus (IFO) for both sides.

### Public Dataset
The public dataset was generated using DWI data sourced from the Human Connectome Project (HCP).

### Local Hospital Dataset
The local hospital dataset was compiled from DWI data provided by the Hospital Clinic of the Medicine College of Ribeirao Preto, University of Sao Paulo (HC FMRP-USP). 

### Preprocessing
Data preprocessing was carried out using MRtrix3 software. The preprocessing pipeline, along with the process of generating tractographies and peak images, is detailed in the "preprocessing" folder. This folder also provides guidance on registering images to a standard space (MNI).

## Code  
The code was developed using Google Colaboratory to enhance readability. The code is organized into four main sections:
1. **Import Libraries:** This section imports the necessary packages for code development and function usage. We used Tensorflow/Keras to construct our model. 
2. **Functions:** Here, you'll find functions tailored to prepare the data for training the U-Net network.
3. **Training:** This section outlines the workflow for calling functions and conducting the training process.
4. **Test and Dice Scores:** Learn how to make predictions using the trained network and calculate Dice scores from the resulting predictions.

## Weights
The "weights" folder contains the best weights obtained during our research training. These weights resulted from training using both the public and local hospital datasets for each tract. You can leverage these weights for predicting new data or for transfer learning purposes.

## Authors, References, Citation and Funding
### Authors and Laboratory
- Hohana Gabriela Konell (hohana.konell@alumni.usp.br)
- Inbrain Lab (inbrain@usp.br)

### Funding
This study received support from the Higher Education Personnel Improvement Coordination (CAPES).

### Citation
If you use something from this repository, please cite us as: 
Konell HG, Junior LOM, Dos Santos AC, Salmon CEG. Assessment of U-Net in the segmentation of short tracts: Transferring to clinical MRI routine. Magn Reson Imaging. 2024 Sep;111:217-228. doi: 10.1016/j.mri.2024.05.009. Epub 2024 May 14. PMID: 38754751.

### Collaboration
We are open to collaborations!! Let's share data and enrich our work!

### Notes
As the public dataset was used through HCP, remember to check the policy of them. 
https://www.humanconnectome.org/

### References 
- Wasserthal, J., Neher, P. & Maier-Hein, K. H. TractSeg - Fast and accurate white matter tract segmentation. Neuroimage 183, 239–253 (2018).
- Wasserthal, J., Neher, P. F., Isensee, F. & Maier-Hein, K. H. Direct White Matter Bundle Segmentation using Stacked U-Nets. Arxiv (2017) doi:10.48550/arxiv.1703.02036.
