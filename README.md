# Retinal-Vessel-Segmentation
## Introduction 
A Coarse-to-Fine Model Structure with Vessel Direction Enhancement for Retinal Vessel Segmentation 
Based on the method from "Study Group Learning: Improving Retinal Vessel Segmentation Trained with Noisy Labels", github repository https://github.com/SHI-Labs/SGL-Retinal-Vessel-Segmentation  
## Methodology 
Our method is based on the Study Group Learning(SGL) method, trying to use the erased labels in SGL model. In the enhancement part, we add a coarse vessel segmentation task and a vessel direction prediction task as the new auxiliary enhancement. In the segmentation part, all the enhancement outputs will be sent into the segmentation module for fine results. So it is a coarse-to-fine model structure. Our changes of the model can improve the vessel segmentation results.  
![our structure](https://github.com/Alexcander-Jing/Retinal-Vessel-Segmentation/blob/main/figs/model%20structure.png)  
## Results 
Our work is performed on the DRIVE and CHASE Dataset, results are as the follows  
