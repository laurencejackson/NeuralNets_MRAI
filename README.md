# Networks for Magnetic Resonance Artificial Intelligence (MRAI)

This is work was performed as part of the MRAI workshop (MIDL 2019 satellite meeting) with exercises designed by Esther Puyol (https://github.com/estherpuyol/MRAI_workshop).

The original networks from the workshop were built using the pytorch library, as a learning exercise I have transferred these to TensorFlow.


# Networks

## LV_segmentation
#### Introduction
Quantitative analysis of cardiac MRI images typically requires a segmentation of the left ventricular (LV) myocardium from the surrounding tissues and  blood pool. This segmentation allows for calculations of useful clinical metrics such as LV ejection fraction, stroke fraction and myocardial mass. However, this segmentation process is often performed manually making it time consuming and susceptible to operator dependent variablility.

#### Objective
Train a neural network to automatically segment the left ventricle from 2D short axis cardiac MR images.

#### Method
A U-net style network was chosen for this problem since it offers 

#### Results
Figure 1 shows the predicted segmentations of the trained network on a sample from the training data. 
<p align="center"><img width="100%" src="./LV_segmentation/imgs/training_data.PNG"><em><br>Figure 1</em></p>

Figure 2 shows the predicted segmentations of the trained network on a sample from the test data. In this case the network is shown to provide useful segmentations from unseen data.
<p align="center"><img width="100%" src="./LV_segmentation/imgs/test_data.PNG"><em><br>Figure 2</em></p>