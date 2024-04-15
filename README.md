# Handwritten Digit Classification (MNIST)

By: @dineshUmasankar

## Introduction

In our digital age, handwritten documents still hold a significant place in our lives. Our daily lives are filled with handwritten letters, legal documents, shopping lists and mathematical equations.

Through the marvels of optical character recognition (OCR), handwritten content has become seamless to convert into various electronic formats. With a simple picture of from our notebook, many of our phones are able to convert our notes into a text file. As our world becomes increasingly connected, the demand for rapid and accurate analysis of physical documents have increased. For Instance, millions of transactions via check are automatically processed via OCR to ensure their accuracy.

Within this project, we explore the seminal paper: "Gradient-Based Learning Applied to Document Recognition", in order to apply various classification methods to recognize handwritten digits \cite{Lecun1998}.

| ![assets/bank-checks.png](assets/bank-checks.png)| 
|:--:| 
| *Reprinted from \cite{BankCheckImage} under fair use and education.* |

#### Background Context

"Real-life document recognition systems are composed of multiple modules including field extraction, segmentation, recognition, and language modeling" \cite{Lecun1998}. Our project will focus mainly on the recognition part of the process. Within the realm of recognition, specifically handwriting recognition (HWR), there are two methods: online and offline.

| ![assets/offline_online.png](assets/offline_online.png)| 
|:--:| 
| *Showcasing offline vs online methodologies of HWR* |

1. **Online methods** - "Online methods involve a digital pen/stylus and have access to the stroke information, pen location while text is being written as seen in the figure [above]. Since they tend to have a lot of information in regard to the flow of text being written they can be classified at a pretty high accuracy and the demarcation between different characters in the text becomes much more clear." \cite{Matcha_2022}.

1. **Offline methods** - "Offline methods involve recognizing text once it's written down and hence won't have information to the strokes/directions involved during writing a possible addition of some background noise from the source [like] paper" \cite{Matcha_2022}. 


To read a bank check, all of these processes must occur to figure out the date of check, payee, amount (in words and numeric form), memo, and signature. This project will focus upon identifying the amount (in numeric form) from a check, where specifically we will build the identification/recognition module to classify the handwritten digits, the amount specified, within a check.

### Problem Statement

> [!NOTE]
> *This problem statement is different from the original project submission due to my own personal interests changing, but the subject area and solution application remain the same.*

**As a user of a bank, I would like to send a picture of my check in order to process the transaction.**

Within this scenario, our bank already has the multiple module system running, except requires a handwritten digit recognition model in order to extract the amount that needs to be transacted between both parties.

As the user will be sending a picture, the project primarily focuses on handwriting recognition via the offline method, and will try to optimize within that in mind.

### Objective

This project can be expanded 

### Motivation


### Significance

