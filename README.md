# Covid Chest X-ray-Detection

## Table of Content
- Introduction
- Architecture
- Dataset
- Motivation
- Installation
- Library Used

### Introduction
![Covid-19-India-and-crisis-communication-1280x720](https://user-images.githubusercontent.com/62636740/91658183-95822980-eae4-11ea-8661-818526f30d67.jpg)

* In December 2019, a new form of coronavirus, SARS-CoV-2, infected humans in Wuhan in the Chinese province of Hubei. The respiratory disease named COVID-19 has become a pandemic that is now spreading very rapidly. Imaging procedures are crucial in the COVID-19 pandemic when it comes to assessing suspected cases and the course of the disease. On the basis of the latest scientific evidence we consider the role of X-ray imaging in the current situation.
* The primary test for diagnosing infection with SARS-CoV-2 is a real-time polymerase chain reaction (RT-PCR) assay of throat swabs or sputum. However, since incubation periods of up to 14 days are possible, in the early stage the possibility of negative RT-PCR findings must be taken into account. In the first few days after the onset of symptoms, computer tomography (CT) can confirm suspected cases and facilitate the prognosis of severe cases. CT captures changes in the lungs of COVID-19 patients at a high rate. This sensitivity can reach 97 percent.

### What Can X-Ray Imaging Do
* Studies of chest X-ray examinations found a lower sensitivity for COVID-19-related lung shadowing of 25 to 69 percent. On the other hand, the ability to identify the disease correctly – the specificity – can be 90 percent. In the studies, all cases of COVID-19 were confirmed with RT-PCR. The low number of participants might have contributed to the discrepancies in sensitivity.
### covid +ve Person X-ray

![covid_chest_x-ray](https://user-images.githubusercontent.com/62636740/91658139-3d4b2780-eae4-11ea-9c54-81fb68f9ae92.jpeg)

### Covid -ve Person X-ray

![normal_xray](https://user-images.githubusercontent.com/62636740/91658165-6966a880-eae4-11ea-9050-059c1bea2ca9.jpg)

### Architecture
### Why are we using ResNet?
* The ResNet has an extremely deep network i.e of 152 layers.
* The shallower version (i.e ResNet50) is available.
* This specialized network architecture was introduced by Microsoft.

### Why does ResNet Perform well?
* Having a regular network which is very deep actually hurts the performance because of vanishing gradient and exploding gradient
* In most of the cases the ResNet's will stop improving rather than decreasing the performance.
* If the layer is not useful L2 regularization will bring its parameters very close to zero.
* The ResNet allows us to converge more faster
* The ResNet's have moderate efficiency depending upon the model and has highest accuracy.

### Full ResNet
![resnet-50](https://user-images.githubusercontent.com/62636740/91658476-1857b400-eae6-11ea-946d-eca62fdd675f.png)
1. It has stacked residual block.
2. Every residual blockc has 3x3 convolution layer.
3. Double layered & the downsample is done spatially using stride of 2 in each dimension.
4. It has an additional convolution layer at the beginning
5. No fully connected layer at the end (only FC 1000 to output class).

### Dataset
You can Download dataset from the [link](https://drive.google.com/drive/folders/1n0x7pVTL3lycztf2kG39rIklKeZNQC4p?usp=sharing)

### Motivation
What to do when you are at home ? I started to learn Machine Learning model to get most out of it. I came to know mathematics behind all supervised models. Finally it is important to work on application (real world application) to actually make a difference.

### Installation
 These code written in [Google Colab](https://www.google.com/search?q=google+colab&oq=google+colab&aqs=chrome..69i57j35i39j0j69i60l5.5070j0j7&sourceid=chrome&ie=UTF-8)
 
### Library

![scikit-learn-logo-small](https://user-images.githubusercontent.com/62636740/91655376-bab76d80-eacd-11ea-8cb1-20ebfd11e7f3.png)

![tensorflow](https://user-images.githubusercontent.com/62636740/91655414-f7836480-eacd-11ea-9b8f-f9eada989d87.jpg)

![keras](https://user-images.githubusercontent.com/62636740/91655424-036f2680-eace-11ea-9aee-d52ddbad3af1.png)
 
