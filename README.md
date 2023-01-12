# Support Vector Machine [![Profile][title-img]][profile]

[title-img]:https://img.shields.io/badge/-SCIA--PRIME-red
[profile]:https://github.com/Pypearl

## Objective

This practical work aims to provide the necessary elements to understand the implementations of a **Support Vector Machine**.

Support Vector Machines (SVMs) are a type of **classification model** used in machine learning. They predict the class of a new example by using a **hyperplane** that separates different classes in the data space.

The goal of SVMs is to find the hyperplane that maximizes the margin between the classes, that is, the distance between the **hyperplane** and the closest examples of each class (called support vectors). This creates a robust and stable prediction model, as it will not be easily influenced by new observations that are not far from the hyperplane.

## Linear SVM

The **optimal gradient** algorithm can be used to efficiently solve the cost function minimization problem of SVMs. It consists of iteratively updating the parameters of the hyperplane using the derivative of the cost function and performing a projection on the domain of the problem's constraints.

It is also possible to solve the SVM problem analytically using the **dual** formulation of the problem. This approach consists of transforming the initial problem into another problem, called the **dual problem**, which can be solved more efficiently. The **dual** formulation allows finding the model parameters by solving a system of linear equations rather than a function minimization problem, which can be faster in some cases. This is what we did in this first part.

## Non-linear SVM

In this second case where the data is not linearly separable, it is not possible to find a hyperplane that perfectly separates the classes. In this case, it is possible to use SVM with **kernels**, which allow transforming the data in a higher dimension space where they can be separated by a hyperplane.

The **kernel trick** is a technique used in conjunction with SVMs to handle non-linearly separable data. It consists of using a **kernel function**, which is a mathematical function that transforms data from one dimension to a higher dimension space so that it is separable by a hyperplane.
