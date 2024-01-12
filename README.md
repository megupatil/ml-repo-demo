# ML Model Management with JFrog Artifactory and JFrog Security Essentials (Xray)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/urasoko/ml-repo-demo/blob/main/demo.ipynb)

## Overview

Use this notebook to experiment with the JFrog Artifactory MLOps feature and the model scanning capabilities for the Hugging Face model hub. 

## Demo

The execution flow of the demo is the following:

* Read configuration file to setup Hugging Face hub via Artifactory
* Block Hugging Face model because it has malicious paclages

## Pre-requisites

1. **ML repo:** create a remote repository on Artifactory for the Hugging Face hub and use the [Set-Me-Up](https://jfrog.com/help/r/jfrog-artifactory-documentation/hugging-face-repositories) to get: repository URL, access token, snippet to resolve models. 
2. **Policy and watch:** Create a JFrog Security Essentials (Xray) [policy](https://jfrog.com/help/r/jfrog-security-documentation/creating-xray-policies-and-rules) to block maliciouspaclages and a watch [watch](https://jfrog.com/help/r/jfrog-security-documentation/configuring-xray-watches) to enforce it on the newly created remote repository.

## Run

1. Open the ```demo.ipynb``` notebook in your preferred ML development environment
2. Run the notebook, Hugging Face models will be resolved via Artifactory
