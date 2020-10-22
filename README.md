<!--
*** Thanks for checking out this README Template. If you have a suggestion that would
*** make this better, please fork the repo and create a pull request or simply open
*** an issue with the tag "enhancement".
*** Thanks again! Now go create something AMAZING! :D
***
***
***
*** To avoid retyping too much info. Do a search and replace for the following:
*** github_username, repo_name, twitter_handle, email
-->





<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]



<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/keyoumao/Credit_Risk">
    <img src="images/logo.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Assess Credit Risk</h3>

  <p align="center">
    Use supervised machine learning to assess the credit risk.
    <br />
    <a href="https://github.com/keyoumao/Credit_Risk"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/keyoumao/Credit_Risk">View Demo</a>
    ·
    <a href="https://github.com/keyoumao/Credit_Risk/issues">Report Bug</a>
    ·
    <a href="https://github.com/keyoumao/Credit_Risk/issues">Request Feature</a>
  </p>
</p>



<!-- TABLE OF CONTENTS -->
## Table of Contents

* [About the Project](#about-the-project)
  * [Built With](#built-with)
* [Getting Started](#getting-started)
* [Usage](#usage)
* [Roadmap](#roadmap)
* [Contributing](#contributing)
* [License](#license)
* [Contact](#contact)
* [Acknowledgements](#acknowledgements)



<!-- ABOUT THE PROJECT -->
## About The Project

[![Product Name Screen Shot][product-screenshot]](https://example.com)

Here's a blank template to get started:
**To avoid retyping too much info. Do a search and replace with your text editor for the following:**
`github_username`, `repo_name`, `twitter_handle`, `email`

In 2019, more than 19 million Americans had at least one unsecured personal loan. That’s a record-breaking number! Personal lending is growing faster than credit card, auto, mortgage, and even student debt. With such incredible growth, FinTech firms are storming ahead of traditional loan processes. By using the latest machine learning techniques, these FinTech firms can continuously analyze large amounts of data and predict trends to optimize lending.

We used Python to build and evaluate several machine learning models to predict credit risk. Being able to predict credit risk with machine learning algorithms can help banks and financial institutions predict anomalies, reduce risk cases, monitor portfolios, and provide recommendations on what to do in cases of fraud.

### Built With

* []()
* []()
* []()



<!-- GETTING STARTED -->
## Getting Started

To get a local copy up and running follow these simple steps.

### Prerequisites

This is an example of how to list things you need to use the software and how to install them.
* npm
```sh
npm install npm@latest -g
```

<!-- USAGE EXAMPLES -->
## Usage

Use this space to show useful examples of how a project can be used. Additional screenshots, code examples and demos work well in this space. You may also link to more resources.

_For more examples, please refer to the [Documentation](https://example.com)_



<!-- ROADMAP -->
## Roadmap

Logistic Regression 
Classification Model Validation 
Support Vector Machines 
Data Preprocessing in Machine Learning 
Decision Trees 
Ensemble Learning and Random Forests 
Bagging and Boosting 


<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.



<!-- CONTACT -->
## Contact

Your Name - [@twitter_handle](https://twitter.com/twitter_handle) - email

Project Link: [https://github.com/keyoumao/Credit_Risk](https://github.com/keyoumao/Credit_Risk)



<!-- ACKNOWLEDGEMENTS -->
## Acknowledgements

* []()
* []()
* []()





<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/github_username/repo.svg?style=flat-square
[contributors-url]: https://github.com/github_username/repo/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/github_username/repo.svg?style=flat-square
[forks-url]: https://github.com/github_username/repo/network/members
[stars-shield]: https://img.shields.io/github/stars/github_username/repo.svg?style=flat-square
[stars-url]: https://github.com/github_username/repo/stargazers
[issues-shield]: https://img.shields.io/github/issues/github_username/repo.svg?style=flat-square
[issues-url]: https://github.com/github_username/repo/issues
[license-shield]: https://img.shields.io/github/license/github_username/repo.svg?style=flat-square
[license-url]: https://github.com/github_username/repo/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/github_username
[product-screenshot]: images/screenshot.png

## Challenge

The goals of this challenge are to:

- Implement machine learning models.
- Use resampling to attempt to address class imbalance.
- Evaluate the performance of machine learning models.
scikit-learn library.
## Tasks

1. Oversample the data using the RandomOverSampler and SMOTE algorithms.
2. Undersample the data using the cluster centroids algorithm.
3. Use a combination approach with the SMOTEENN algorithm.
For each of the above:

    1. Train a logistic regression classifier (from Scikit-learn) using the resampled data.
    2. Calculate the balanced accuracy score using balanced_accuracy_score from sklearn.metrics.
    3. Generate a confusion_matrix.
    4. Print the classification report (classification_report_imbalanced from imblearn.metrics).

## Analysis

### Oversampling

#### Naive Random Oversampling

The accuracy score for the random oversampling is 0.65.The classification report is given as follows. The precision for high_risk is 0.01, very low and high for the low risk, indicating an overfitting for the low_risk. The recall (sensitivity) for both cases are not ideal.

                   pre       rec       spe        f1       geo       iba       sup

    high_risk       0.01      0.70      0.60      0.02      0.65      0.42       101
    low_risk       1.00      0.60      0.70      0.75      0.65      0.42     17104

    avg / total       0.99      0.60      0.70      0.74      0.65      0.42     17205

#### SMOTE Oversampling

The accuracy score for the SMOTE oversampling is 0.63.The classification report is given as follows. The precision for high_risk is 0.01, very low and high for the low risk, indicating an overfitting for the low_risk. The recall (sensitivity) for both cases are not ideal and lower than the random oversampling.

                   pre       rec       spe        f1       geo       iba       sup

    high_risk       0.01      0.59      0.66      0.02      0.62      0.39       101
    low_risk       1.00      0.66      0.59      0.79      0.62      0.39     17104

    avg / total       0.99      0.66      0.59      0.79      0.62      0.39     17205

To sum up, the oversampling cases are not good.

### Undersampling

The accuracy score for the random oversampling is 0.63.The classification report is given as follows. The precision for high_risk is 0.01, very low and high for the low risk, indicating an overfitting for the low_risk. The recall (sensitivity) for both cases are not good.

                   pre       rec       spe        f1       geo       iba       sup

    high_risk       0.01      0.65      0.54      0.02      0.60      0.36       101
    low_risk       1.00      0.54      0.65      0.70      0.60      0.35     17104

    avg / total       0.99      0.54      0.65      0.70      0.60      0.35     17205

### Combination (Over and Under) Sampling

The accuracy score for the random oversampling is 0.6.The classification report is given as follows. The precision for high_risk is 0.01, very low and high for the low risk, indicating an overfitting for the low_risk. The recall (sensitivity) for both cases are not good.

                   pre       rec       spe        f1       geo       iba       sup

    high_risk       0.01      0.70      0.60      0.02      0.65      0.43       101
    low_risk       1.00      0.60      0.70      0.75      0.65      0.42     17104

    avg / total       0.99      0.60      0.70      0.75      0.65      0.42     17205

## Recommendations

From the analysis above, all of the models above are not recommended. Because all the models have accuracy scores less than 0.7. The precision score for the credit scores are overfit apparently. The recall (sensitivity) is also not good. More detailed model to distinguish the features need to be establlished for a better prediction.

## Extension

BalancedRandomForestClassifier improved the accuracy score a little bit to 0.74. But the precision and sensitivity still exist. EasyEnsembleClassifier is by far the best model, where the accuracy score is 0.94. The sensitivity has been improved as well. The classification_report_imbalanced is given as follows.

                   pre       rec       spe        f1       geo       iba       sup

    high_risk       0.10      0.92      0.95      0.18      0.94      0.87       101
    low_risk       1.00      0.95      0.92      0.97      0.94      0.88     17104

    avg / total       0.99      0.95      0.92      0.97      0.94      0.88     17205
