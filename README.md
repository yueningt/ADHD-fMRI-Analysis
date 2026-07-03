# ADHD-fMRI-Analysis
A Convolutional Neural Network (CNN) to analyze fMRIs of control and ADHD subjects

## The Data

The dataset used in this project is publicly available on OpenNeuro. It investigates the neural mechanisms of working memory and reward processing in children diagnosed with Attention Deficit Hyperactivity Disorder (ADHD) compared to typically developing controls.

### Dataset Citation
If you use this data or code in your research, please cite the original dataset:

> Booth, J. R., Cooke, G. E., Gayda, J., Hammer, R., Lytle, N. M., Stein, M. A., & Tennekoon, M. (2021). *Working Memory and Reward in Children with and without Attention Deficit Hyperactivity Disorder (ADHD)*. OpenNeuro. [Dataset] https://doi.org

### Accessing the Dataset
The 47 GB raw imaging folder is not stored directly in this GitHub repository due to file size constraints. You can access and download the full dataset using any of the following methods:

* **Direct Web Download:** Visit the repository directly on [OpenNeuro (ds002424)](https://openneuro.org).
* **OpenNeuro CLI:** Download via the command line tool:
  ```bash
  openneuro download --dataset ds002424
  ```

### Structure
The data follows the **Brain Imaging Data Structure (BIDS)** standard. Ensure the downloaded `ds002424` folder is placed in the root directory of this project before running any preprocessing or analysis scripts.

James R. Booth, GE Cooke, Jessica Gayda, Rubi Hammer, Marisa N. Lytle, MA Stein, and Michael Tennekoon (2021). Working Memory and Reward in Children with and without Attention Deficit Hyperactivity Disorder (ADHD). OpenNeuro. [Dataset] doi: 10.18112/openneuro.ds002424.v1.2.0

## The Code
The ADHD CNN Model.ipynb notebook contains the core pipeline for the Convolutional Neural Network (CNN). This script automatically loads the raw neuroimaging data from the ds002424 directory, executes the required preprocessing steps, and feeds the processed images into a custom-built CNN architecture. Following model optimization, the network visualizes and outputs the key diagnostic features (activation maps) used by the algorithm to differentiate between ADHD and control subjects.

## Findings
Detailed documentation of the model’s performance, data interpretation, and clinical implications can be found in Model Methods-Conclusion.docx. This document provides a comprehensive analysis of the results, detailing how the model-extracted features map to underlying neurological patterns and evaluating their overall statistical and practical significance.
