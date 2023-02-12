# `PR104`

### Reproduction of a Software Quality Prediction Study

*Comparison of Machine Learning Techniques for Software Quality Prediction*
<br>
a paper by **Goyal, S. (2020)** published in *Int. J. Knowl. Syst. Sci.*, **11(2)** - 
[IGI Global](https://www.igi-global.com/article/comparison-of-machine-learning-techniques-for-software-quality-prediction/252885)

***

This repository contains the reproduction of a small paper on software quality prediction as a university project. The original paper provides an overview of different software quality prediction models and their performance in terms of accuracy, recall and ROC AUC. The goal of this reproduction project is to validate the findings of the original paper, provide a deeper understanding of the various software quality prediction models, and to critically evaluate the approach and choices made by the authors.

The work utilizes data collected from NASA projects using McCabe metrics which are made available in the [PROMISE repository](http://promise.site.uottawa.ca/SERepository/index.html). This research is done with six fault prediction benchmark datasets named `CM1`, `KC1`, `KC2`, `PC1`, `JM1`, and `ALL_DATA` (a combination of the previous datasets). The data has been collected using McCabe and Halstead features extractors from the source code of multiple projects.

The repository includes all the necessary code and data to reproduce the study, as well as a collection of the utility functions used in the analysis. The results obtained from the reproduction are also included, allowing for easy comparison with the original study. 
The `data` folder contains the project data, the `ref` folder contains the project paper and the `scripts` folder contains notebooks in which the analysis is carried out and explained along with the setup and utility functions used.

In addition to reproducing the paper, this repository also critiques the approach taken by the authors. One major criticism is that the authors did not properly handle the class imbalance problem, which can greatly impact the performance of the models. Furthermore, the authors used misleading and inadequate performance metrics, which also affected the conclusions of the results.

If you are interested in software quality prediction or simply want to learn about the different models and techniques used in this field, this repository is for you! The code is well documented and easy to follow, making it an excellent resource for anyone looking to get started with software quality prediction. In addition, the critical evaluation of the original paper provides valuable insight into the limitations and potential improvements in this field of research.

So feel free to take a look, experiment with the code, and let me know if you have any questions or suggestions!

***
