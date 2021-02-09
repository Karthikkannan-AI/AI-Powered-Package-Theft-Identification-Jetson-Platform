# AI powered Package Theft Identification (Jetson Platform) #

## Table of Contents ##

* [Introduction](https://github.com/Karthikkannan-AI/Package-AI#introduction)
* [The Problem](https://github.com/Karthikkannan-AI/Package-AI#problem)
  * [Analysis of the Problem ](https://github.com/Karthikkannan-AI/Package-AI#analysis-of-the-problem)
  * [Package Thefts (Facts)](https://github.com/Karthikkannan-AI/Package-AI#package-thefts-facts)
* [Solution](https://github.com/Karthikkannan-AI/Package-AI#proposed-solution)
  * [Solution Workflow](https://github.com/Karthikkannan-AI/Package-AI#solution-workflow)
  * [Evaluation of the Solution](https://github.com/Karthikkannan-AI/Package-AI#evaluation-of-the-solution)
* [Conclusion](https://github.com/Karthikkannan-AI/Package-AI#conclusion)
* [References](https://github.com/Karthikkannan-AI/Package-AI#references)
* [Contact Us](https://github.com/Karthikkannan-AI/Package-AI#contact-us)


## Introduction ##

Online shopping has reached an all-time high due to the coronavirus pandemic and there is a huge surge in Package Theft (package left on the door by the delivery personnel ). We have built a Proof of Concept of identifying the Package from the real-time CCTV stream when it arrives/ placed on the door side and intimates the house owner if the Package is taken away. (  __ALARM__ is triggered )


## Problem ##

In this particular demonstration we will focus on the package theft problem in USA. Around 1.7 million packages are stolen or go missing every day in USA, accounting to a lost revenue of $25 million per day or $9 billion per year.


### Analysis of the Problem ###


<p float-"left">
<img src="https://github.com/Karthikkannan-AI/Package-AI/blob/main/resources/p.png" width="49%">

<img src="https://github.com/Karthikkannan-AI/Package-AI/blob/main/resources/p0.png" width="50%">
</p>

<img src="https://github.com/Karthikkannan-AI/Package-AI/blob/main/resources/p1.png" width="100%"/>


### Package Thefts (Facts) ###

<img src="https://github.com/Karthikkannan-AI/Package-AI/blob/main/resources/p2.png" width="70%">


## Proposed Solution ##

### Solution Workflow ###

<img src="https://github.com/Karthikkannan-AI/Package-AI/blob/main/resources/p3.jpg" width="70%">

To arrive at the Solution, we have to go through 5 Major Steps


| Step Numbers | Procedures | Definitions |
| :--------------: | :--------------: | :--------------: |
| Step 1   | Data Preparation | Collect thousands of Images of Delivery Box ( Different shape, size and environment) to mimic the real. |
| Step 2   | Data Annotation | As we have planned to do object detection, we have to annotate those images with Bounding Boxes. |
| Step 3   | Training | The Images are Trained using NVIDIA TLT. |
| Step 4   | Evaluation | The custom Deep Learning Model is Tested and Evaluated. If there are issues with the detection accuracy in specific conditions then we have to retrain the model by taking in to consideration those scenarios. |
| Step 5   | Deployment | IP CCTV camera is connected to Nano through RTSP. If the CCTV Feed identifies the Delivery Box, immediately through SMTP a mail is triggered to the House Owner. If the RTSP Stream doesn’t identify the Delivery Box, the prior 20 sec frame is taken and converted in to a video and sent as email to the House Owner , so that we can know the theft event. |


### Evaluation of the Solution ###

 __Test - 1__



<a href="http://www.youtube.com/watch?feature=player_embedded&v=https://youtu.be/lvhZhcscF74" target="_blank"><img src="https://github.com/Karthikkannan-AI/Package-AI/blob/main/resources/tns/po1.png" 
alt="Package AI - Test 1" width="75%"  /></a> 


 __Test - 2__



<a href="http://www.youtube.com/watch?feature=player_embedded&v=https://youtu.be/-t-ZHlzPdNs" target="_blank"><img src="https://github.com/Karthikkannan-AI/Package-AI/blob/main/resources/tns/po2.png" 
alt="Package AI - Test 2" width="75%" /></a> 


 __Test - 3__



<a href="http://www.youtube.com/watch?feature=player_embedded&v=https://youtu.be/1pAiANJmDKY" target="_blank"><img src="https://github.com/Karthikkannan-AI/Package-AI/blob/main/resources/tns/po3.png" 
alt="Package AI - Test 3" width="75%" /></a> 


__Test - 4__



<a href="http://www.youtube.com/watch?feature=player_embedded&v=https://youtu.be/hpNYHv-9KCM" target="_blank"><img src="https://github.com/Karthikkannan-AI/Package-AI/blob/main/resources/tns/po4.png" 
alt="Package AI - Test 4" width="75%" /></a>


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
