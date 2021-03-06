# Coronavirus Disease Analysis using Chest X-Ray Images and a Novel Deep Convolutional Neural Network
The recent emergence of a highly infectious and contagious respiratory viral disease known as COVID-19 has vastly impacted human lives and greatly burdened the health care system. Therefore, it is indispensable to develop a fast and accurate diagnostic system for timely identification of COVID-19 infected patients and to control its spread. This work proposes a new X-ray based COVID-19 classification framework consisting of (i) end-to-end classification module and (ii) deep feature-space based Machine Learning classification module. In this regard, two new custom CNN architectures, namely COVID-RENet-1 and COVID-RENet-2 are developed for COVID-19 specific pneumonia analysis by systematically employing Region and Edge base operations along with convolution operations. The synergistic use of Region and Edge based operations explores the region homogeneity, textural variations and region boundary; it thus helps in capturing the pneumonia specific pattern. In the first module, the proposed COVID-RENets are used for end-to-end classification. In the second module, the discrimination power is enhanced by jointly providing the deep feature hierarchies of the COVID-RENet-1 and COVID-RENet-2 to SVM for classification. The discrimination capacity of the proposed classification framework is assessed by comparing it against the standard state-of-the-art CNNs using radiologist’s authenticated chest X-ray dataset. The proposed classification framework shows good generalization (accuracy: 98.53%, F-score: 0.98, MCC: 0.97) with considerable high sensitivity (0.99) and precision (0.98). The exemplary performance of the classification framework suggests its potential use in other X-ray imagery based infectious disease analysis.

In this repository, we provide the MATLAB GUI and Testing Code for the Coronavirus Disease Analysis using Chest X-ray Images for the research community to use our research work

**Overview of the workflow for the proposed COVID-19 Classification Framework**
In this work, a new classification framework is developed based on deep learning and classical ML techniques for automatic discrimination of COVID-19 infected patients from healthy individuals based on chest X-ray images. The proposed classification framework is constituted of two modules: (i) Proposed COVID-RENet based end-to-end Classification, and (ii) Deep Concatenated Feature-space based ML classification. In the experimental setup, initially, training samples were augmented to improve the generalization. These augmented samples were used to train the two proposed modules. Fig. 1. (A) shows the modules of the proposed COVID-19 classification framework, whereas (B) gives the detailed overview of the workflow.


![workflow](https://user-images.githubusercontent.com/87992381/127025469-32b88253-9f5f-401f-8efc-0618d92783ce.png)


**Table**
|Backbone |Style|	Lr schd |	Mem (GB)|	Inf time (fps)|	box AP	|
|---------:|----:|--------:|--------:|--------------:|--------:|
|R-50-FPN|	caffe	|	4.3	|	                |38.0|	34.4|
|R-50-FPN|	pytorch	|	4.4|	16.1|38.2|	34.7|

