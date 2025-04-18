# Semi-Supervised-Domain-Adaptation-SSDA-with-Correlation-Alignment-CORAL-
Semi-Supervised Domain Adaptation (SSDA) with Correlation Alignment (CORAL). In this Tutorial we are using  MNIST(Source Domain) and SVHN (Target Domain) datasets


Overview of CORAL

CORrelation ALignment (CORAL) loss is a technique used in domain adaptation to align the second-order statistics (covariances) of the source and target domain features. The goal is to reduce the domain shift by matching the covariance matrices of the two domains.

Importance of CORAL You need a simple and efficient alignment technique.You want to integrate alignment into deep learning models easily, then it would be with other alignment techniques like MMD (Maximum Mean Discrepancy)

Semi-Supervised Learning In a semi-supervised setting, you have a mixture of labeled and unlabeled data in the target domain.

Applications of Coral in SSDA This scenario is quite common as it benefits from both the alignment of feature distributions and the utilization of limited labeled target data to enhance adaptation.

Data Preparation

In this tutorial, SVHN will be our target domain and MNIST will be our source domain

SVHN (Real-World Dataset): Contains real-world images of house numbers,
making it a challenging and practical dataset.

MNIST Contains grayscale images of handwritten digits, providing a controlled environment for experimentation.

![image](https://github.com/user-attachments/assets/3546af4b-6046-4a99-a2b7-c90122697271)


CORAL Alignment:

A CORAL loss term is added to the overall loss function of the model. This loss term measures the difference between the source and target covariance matrices. The model is trained to minimize this loss, encouraging the feature distributions to align.


Feature Extraction

By integrating CORAL with a feature extractor like ResNet, you can effectively align the feature distributions of the source and target domains, improving the model's performance on the target domain.
