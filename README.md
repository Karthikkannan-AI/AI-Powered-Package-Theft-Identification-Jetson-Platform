# Package-AI

## Table of Contents ##

* Introduction 
* The Problem
  * Analysis of the Problem 
  * Package Thefts (Facts)
* Solution 
  * Solution Workflow
  * Evaluation of the Solution
* Conclusion
* References
* Contact Us


## Introduction ##

Online shopping has reached an all-time high due to the coronavirus pandemic and there is a huge surge in Package Theft across America. 
We have built a Proof of Concept of converting a CCTV camera in the door in to an AI Powered Camera using NVIDIA Jetson Platform to Identify the Package when it arrives/ placed on the door side and intimates the house owner, if the Package is taken away the __ALARM__ is triggered 


## Problem ##

We will look how serious and widespread the Package theft Problem is in USA. 
Around 1.7 million packages are stolen or go missing every day in USA, accounting to a lost revenue of $25 million per day or $9 billion per year

<p float-"left">
<img src="https://github.com/Karthikkannan-AI/Package-AI/blob/main/resources/p.png" width="49%">

<img src="https://github.com/Karthikkannan-AI/Package-AI/blob/main/resources/p0.png" width="50%">
</p>


### Analysis of the Problem ###

<img src="https://github.com/Karthikkannan-AI/Package-AI/blob/main/resources/p1.png" width="70%"/>


### Package Thefts (Facts) ###

<img src="https://github.com/Karthikkannan-AI/Package-AI/blob/main/resources/p2.png" width="70%">


## Solution ##

### Solution Workflow ###

<img src="https://github.com/Karthikkannan-AI/Package-AI/blob/main/resources/p3.jpg" width="70%">

To arrive at the Solution, we have to go through 5 Major Steps

__Step 1 : Data Preparation__

Collect thousands of Images of Delivery Box ( Different shape, size and environment) to mimic the real.

__Step 2 : Data Annotation__

As we have planned to do object detection, we have to annotate those images with Bounding Boxes.

__Step 3 : Training__

The Images are Trained using NVIDIA TLT.

__Step 4 : Evaluation__

The custom Deep Learning Model is Tested and Evaluated. If there are issues with the detection accuracy in specific conditions then we have to retrain the model by taking in to consideration those scenarios.

__Step 5 : Deployment__

IP CCTV camera is connected to Nano through RTSP. 

If the CCTV Feed identifies the Delivery Box, immediately through SMTP a mail is triggered to the House Owner. 

If the RTSP Stream doesn’t identify the Delivery Box, the prior 20 sec frame is taken and converted in to a video and sent as email to the House Owner , so that we can know the theft event


### Evaluation of the Solution ###




## Conclusion ##

* We have built this as a Proof of Concept to showcase how we can build a custom deep learning Model to solve a Package theft problem using computer vision. 
* We have provided the Model, which can be tested for its real world performance. 
* We have considered only carton boxes of different shapes and size for Package, Further works are required to improve the detection accuracy with various other packages other than carton boxes 


## References ##

1. https://www.security.org/resources/stolen-packages-survey/
2. https://www.cnbc.com/2020/01/10/package-theft-how-amazon-google-others-are-fighting-porch-pirates.html
3. https://www.nytimes.com/2019/12/02/nyregion/online-shopping-package-theft.html


## Contact Us ##

__ETOP TECHNOLOGIES__ is a Software Development company.

1. We do AI Consulting for Digital Transformation.
2. We build software solutions using emerging technologies for start-ups and enterprises.
3. We can Develop AI applications with Computer vision, Deep Learning and Natural Language processing.


We convert your AI Vision into a reality. Our Services are categorized into

1. AI Data Preparation/ Data Annotation Services
2. AI Software Development Services
3. AI IOT Development Services

__Visit www.etopdigital.com for more information.__

<br><br>
<img src="https://github.com/Karthikkannan-AI/Package-AI/blob/main/resources/About%20ETOP%20Technologies_Github.png">
