# Short Tracts Automatic Sementation
In this repository you will find the code, weights and data for automatic segmention of shor tracts such as anterior, posterior and hippocampal comissure, fornix and uncinated fascículus. 

## Data
This repository contains two datasets: public dataset and local hospital dataset. 
Both datasets contains train (n=100), validation (n=15) and test (n=60) images, composed by peaks images (input) and binary masks (output/ground truth).

The binary masks are from 11 different tracts, 5 short tracts: Anterior Commissure (AC), Posterior Commissure (PC), Hippocampal Commissure (HC), Fornix (FX) left and right and Uncinated Fascículus (UF) left and right. And 2 long tracts: Cortical Spinal Tract (CST) and Inferior Front-Occipital Fascículus (IFO) left and right. 

### Public Dataset
The public dataset were generated through DWI data provided by the Human Connectome Project (HCP).
### Local Hospital Dataset
The local hospital data were generated through DWI data provided by the Hospital Clinic of the Medicine College of Ribeirao Preto from University of Sao Paulo (HC FMRP-USP). 

## Autors, references and funding
### Autors and laboratory
* Hohana Gabriela Konell (hohana.konell@usp.br)
* Inbrain Lab (inbrain@usp.br)
### Funding
This study was supported by Higher Education Personnel Improvement Coordination (CAPES). 
### References 
Wasserthal, J., Neher, P. & Maier-Hein, K. H. TractSeg - Fast and accurate white matter tract segmentation. Neuroimage 183, 239–253 (2018).
Wasserthal, J., Neher, P. F., Isensee, F. & Maier-Hein, K. H. Direct White Matter Bundle Segmentation using Stacked U-Nets. Arxiv (2017) doi:10.48550/arxiv.1703.02036.
