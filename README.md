# Machine Vision System for Inspecting Weld Quality on Stainless Steel using HDR Cameras and Deep Learning
## ML and NN 1st Project

### Notebooks
***Title: TIG Welding Defects Classification Notebooks***

***Description: This section contains Jupyter notebooks for TIG welding defects classification.***

***Repository: [GitHub - TIG Welding Defects Classification Notebooks](https://github.com/SamuelK87/Machine-vision-based-defect-detection-in-welding-process)***

***Author: haarshit20***

***Accessed Date: January 2, 2024***

### Dataset
***Tittle: Tig Stainless Steel 304 Dataset***

***Description: This dataset contains information on Tig welding of stainless steel 304.***

***Source: [Kaggle - Tig Stainless Steel 304 Dataset](https://www.kaggle.com/datasets/danielbacioiu/tig-stainless-steel-304)***

***Author: Daniel Bacioiu***

***Publication Year: (Publication year, if available)***

***Accessed Date: January 2, 2024***

## Summary of Method:
This paper presents the development and evaluation of a machine vision system with **Python in Jupyter Notebook** for inspecting weld quality on stainless steel using HDR cameras and deep learning. The system employed a transfer learning approach, leveraging a pre-trained VGG16 convolutional neural network (CNN) for feature extraction and adapting it to the specific task of weld defect classification.

### Key Steps:
#### Data Acquisition and Preprocessing:
Captured a dataset of high-quality HDR images of stainless steel welds under controlled and varied welding conditions.
Labeled the images according to weld quality (good/defective) and specific defect types (burn-through, contamination, lack of fusion, etc.).
Applied image pre-processing techniques like normalization and random transformations (cropping, flipping, rotation) to enhance data diversity and improve model generalizability.

![image](https://github.com/user-attachments/assets/5b30e2e5-bcca-48c8-b977-9a96e072ea94)


#### Transfer Learning with VGG16:
Used a pre-trained VGG16 model, known for its strong image feature extraction capabilities.
Froze the initial layers of VGG16 to preserve its pre-trained weights and prevent overfitting.
Replaced the final classification layer of VGG16 with a new layer specific to the six weld defect classes.
Trained the modified VGG16 model on the labeled weld image dataset.

#### Evaluation and Analysis:
Evaluated the trained model on a separate test dataset of unseen weld images.
Measured performance using various metrics, including accuracy, precision, recall, F1-score, and confusion matrix.
Analyzed the model's strengths and weaknesses for different defect types.

#### Highlights:
The transfer learning approach with VGG16 achieved a high test accuracy of 93% in classifying weld defects on stainless steel.
Precision scores were generally high for most defect types, demonstrating the model's ability to correctly identify defects.
Recall scores were excellent for "good weld," "burn through," and "lack of fusion" defects, indicating strong detection performance for these critical classes.

The F1-score, which balances precision and recall, was also high for "good weld" and "lack of fusion" defects, confirming the model's robust performance for these categories.

This study demonstrates the promising potential of using HDR cameras and transfer learning with deep learning models for automated and accurate weld defect inspection on stainless steel.

### References
Automated defect classification of Aluminium 5083 TIG welding using HDR camera and neural networks (Daniel Bacioiua, Geoff Melton, Mayorkinos Papaeliasa, Rob Shaw)

Automated defect classification of SS304 TIG welding process using visible spectrum camera and machine learning (Bacioiu, Daniel; Melton, Geoff; Papaelias, Mayorkinos; Shaw, Rob)

W. Lucas, D. Bertaso, G. Melton, J. Smith, and C. Balfour. Real-time vision-based control of weld pool size. Welding International, 26(4):243–250, 2012.

J. Mirapeix, P.B. Garca-Allende, A. Cobo, O.M. Conde, and J.M. L´opez-Higuera. Real-time arc-welding defect detection and classification with principal component analysis and artificial neural networks. {NDT} & E International, 40(4):315 – 323, 2007.

H.S. Song and Y.M. Zhang. Three-dimensional reconstruction of specular surface for a gas tungsten arc weld pool. Measurement Science and Technology, 18(12):3751, 2007.

Y. Ou and Y. Li. Quality evaluation and automatic classification in resistance spot welding by analyzing the weld image on metal bands by computer vision. International Journal of Signal Processing, Image Processing and Pattern Recognition, 8:301–314, 05 2015.
