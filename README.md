# Handwritten Digit Classification (MNIST)

By: Dinesh Umasankar

## Introduction

In our digital age, handwritten documents still hold a significant place in our lives. Our daily lives are filled with handwritten letters, legal documents, shopping lists and mathematical equations.

Through the marvels of optical character recognition (OCR), handwritten content has become seamless to convert into various electronic formats. With a simple picture of from our notebook, many of our phones are able to convert our notes into a text file. As our world becomes increasingly connected, the demand for rapid and accurate analysis of physical documents have increased. For Instance, millions of transactions via check are automatically processed via OCR to ensure their accuracy.

Within this project, we explore the seminal paper: "Gradient-Based Learning Applied to Document Recognition", in order to apply various classification methods to recognize handwritten digits \cite{Lecun1998}.

### Background Context

"Real-life document recognition systems are composed of multiple modules including field extraction, segmentation, recognition, and language modeling" [@Lecun1998]. Our project will focus mainly on the recognition part of the process. Within the realm of recognition, specifically handwriting recognition (HWR), there are two methods: online and offline.

| ![assets/offline_online.png](assets/offline_online.png)| 
|:--:| 
| *Showcasing offline vs online methodologies of HWR* [@Jayadevan2011] |

1. **Online methods** - "Online methods involve a digital pen/stylus and have access to the stroke information, pen location while text is being written as shown in the figure. Since they tend to have a lot of information in regard to the flow of text being written they can be classified at a pretty high accuracy and the demarcation between different characters in the text becomes much more clear" [@Matcha_2022].

1. **Offline methods** - Offline methods involve recognizing text once it's written down and thus won't have information to the strokes/directions involved during writing, however, it will also have the addition of some background noise such as paper and shadows [@Matcha_2022].


This project will focus on following the applications mentioned in the seminal paper, where we will build an identification/recognition module to read a bank check. All the processes within document recognition must occur to read a bank check's various components: date, payee, amount (in word form), amount (in numeric form), and signature. Due to time constraints, we will focus only building the module to classify the handwritten digits within the amount specified field of a check, and leave the rest of the implementation to our readers as our approach can be extended to the other fields as well.

### Problem Statement

> [!NOTE]
> *This problem statement is slightly different from the original project submission due to my own personal interests changing, but the subject area and solution application remain the same. The focus has shifted from online HWR method from a pen computer into an offline HWR method.*

**As a user of a bank, I would like to send a picture of my check in order to process a transaction.**

Within this scenario, our hypothetical bank already has the multiple module system running, except they require a handwritten digit recognition model in order to extract the amount that needs to be transacted between both parties.

As the user will be sending a picture, the project will primarily focus on handwriting recognition via the offline method.

### Objective

Build out an identification / recognition module for the amount (in numeric form) field from a check to classify handwritten digits in the context of a bank check reader application within a hypothetical bank.

### Motivation

There are numerous physical forms and papers, and building out the digit classification system could further digital transformation of existing businesses and industries. By digitizing, it opens up a whole new array of possibilities to analyze at depth for any company, such as being able to feed the information into a Retrieval-Augmented Generation (RAG) model to extract key insights. Furthermore, it would be the first stepping stone to build a generalized OCR system that can be applied regardless of context.

### Significance

The significance of this project is to showcase the ability to convert physical documents into electronic format(s), which would increase one's capability to search and retrieve, and possibly generate new content, especially in our modern day of generative artificial intelligence. The principle(s) of this project can be applied into any application-specific or industry-specific instance to provide key insights or accelerate existing processes.

### Related Work

There are numerous previous works who have delved into classifying handwritten digits, specifically from the MNIST Dataset. From the seminal paper in 1998, Yann Lecun's team had created LeNet-5, a convolutional neural network (CNN), which had achieved an accuracy of over 98%. In addition, their team had also compared various other classification methods, notably, they used a support vector machine (SVM) that used the polynomial kernel that also achieved accuracies of over 98% [@Lecun1998]. As of now, 35 years after the seminal paper, the highest accuracy recorded is 99.87% achieved through an ensemble of Homogeneous Vector Capsules (HVCs) that also optimizes on the number of parameters and required amount of training epochs [@Byerly2020]. Throughout that time, most of the further experimentation to improve accuracies have still relied on the fundamental principle(s) of utilizing deep learning to solve this problem, and still use the base essence of CNNs (either in ensemble or combined into different architectures) to achieve higher accuracies.

In terms of the scope of this project, (and what I personally understand), I will tackle this problem from the classification algorithms taught within my undergraduate education and my preliminary research into the subject field. We will utilize logarithmic regression, SVMs, Decision Tree, Random Forest, and multilayer perceptrons with various activation function(s).
