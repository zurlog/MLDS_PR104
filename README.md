# `PR104`
[![Made withJupyter][jupyter-shield]][jupyter-url]
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Issues][issues-shield]][issues-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

### Reproduction of a Software Quality Prediction Study

*Comparison of Machine Learning Techniques for Software Quality Prediction*
<br>
a paper by **Goyal, S. (2020)** published in *Int. J. Knowl. Syst. Sci.*, **11(2)** - 
[IGI Global](https://www.igi-global.com/article/comparison-of-machine-learning-techniques-for-software-quality-prediction/252885)

***

This repository contains the reproduction of a small paper on software quality prediction as a university project. The original paper provides an overview of different software quality prediction models and their performance in terms of accuracy, recall and ROC AUC. The goal of this reproduction project is to validate the findings of the original paper, provide a deeper understanding of the various software quality prediction models, and to critically evaluate the approach and choices made by the authors.

In addition to reproducing the paper, this repository also critiques the approach taken by the authors. One major criticism is that the authors did not properly handle the class imbalance problem, which can greatly impact the performance of the models. Furthermore, the authors used misleading and inadequate performance metrics, which also affected the conclusions of the results.

If you are interested in software quality prediction or simply want to learn about the different models and techniques used in this field, this repository is for you! The code is well documented and easy to follow, making it an excellent resource for anyone looking to get started with software quality prediction. In addition, the critical evaluation of the original paper provides valuable insight into the limitations and potential improvements in this field of research.

So feel free to take a look, experiment with the code, and let me know if you have any questions or suggestions!

<br>


## Data
The work utilizes data collected from NASA projects using McCabe metrics which are made available in the [PROMISE repository](http://promise.site.uottawa.ca/SERepository/index.html). This research is done with six fault prediction benchmark datasets named `CM1`, `KC1`, `KC2`, `PC1`, `JM1`, and `ALL_DATA` (a combination of the previous datasets). The data has been collected using McCabe and Halstead features extractors from the source code of multiple projects.
<br>

| Name | Instances | Buggy | Clean | Imbalance Ratio | Features | Source |
| ---- | --------- | ----- | ----- | --------------- | ------- | ------ |
| CM1  | 498       | 49    | 449   | 0.109          | 22      | CM1 is a NASA spacecraft instrument written in C |
| JM1  | 10885     | 2106  | 8779  | 0.240          | 22      | JM1 is written in C and is a real-time predictive ground system. It uses simulations to generate predictions |
| KC1  | 2109      | 326   | 1783  | 0.183          | 22      | KC1 is a C++ system implementing storage management for receiving and processing ground data |
| KC2  | 522       | 107   | 415   | 0.258          | 22      | C++ functions used in a scientific data project which is separate from another part known as KC1. These share some third-party software libraries with no other software overlap |
| PC1  | 1109      | 77    | 1032  | 0.075          | 22      | Data from C functions. Flight software for earth orbiting satellite |
| ALL_DATA | 15123 | 2665  | 12458 | 0.214          | 22      | Combined Dataset |


<br>

## Usage
The repository includes the code, data, and results necessary to reproduce the study. The `data` folder holds the benchmark datasets, the `ref` folder contains the original research paper, and the `scripts` folder holds the Jupyter notebooks for the analysis and setup of utility functions. The results from the reproduction are also provided in the `results` folder for an easy comparison with the original study.

<br>
<br>


## Acknowledgments
*References, Inspiration, Code Snippets, etc.*

* [Goyal, S. (2020)](https://www.igi-global.com/article/comparison-of-machine-learning-techniques-for-software-quality-prediction/252885)
* [Goyal, S. (2022) **Handling Class-Imbalance with KNN (Neighbourhood) Under-Sampling for Software Defect Prediction**. *Artif Intell Rev 55, 2023–2064*](https://link.springer.com/article/10.1007/s10462-021-10044-w)
* [Kan, S. H. (2003) **Metrics and Models in Software Quality Engineering**. *Addison-Wesley Professional, 2003*](https://books.google.it/books/about/Metrics_and_Models_in_Software_Quality_E.html?id=EaefcL3pWJYC&redir_esc=y)
* [Nested versus non-nested cross-validation](https://scikit-learn.org/stable/auto_examples/model_selection/plot_nested_cross_validation_iris.html#sphx-glr-auto-examples-model-selection-plot-nested-cross-validation-iris-py)
* [Receiver Operating Characteristic (ROC) with cross validation](https://scikit-learn.org/stable/auto_examples/model_selection/plot_roc_crossval.html#sphx-glr-auto-examples-model-selection-plot-roc-crossval-py)

***

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/zurlog/dpc-covid19.svg?style=for-the-badge
[contributors-url]: https://github.com/zurlog/dpc-covid19/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/zurlog/dpc-covid19.svg?style=for-the-badge
[forks-url]: https://github.com/zurlog/dpc-covid19/network/members
[issues-shield]: https://img.shields.io/github/issues/zurlog/dpc-covid19.svg?style=for-the-badge
[issues-url]: https://github.com/zurlog/dpc-covid19/issues
[license-shield]: https://img.shields.io/github/license/zurlog/dpc-covid19.svg?style=for-the-badge
[license-url]: https://github.com/zurlog/dpc-covid19/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/zurlogiovanni/
[product-screenshot]: images/screenshot.png
[jupyter-shield]: https://img.shields.io/badge/Made%20with-Jupyter-orange?style=for-the-badge&logo=Jupyter
[jupyter-url]: https://jupyter.org/try
