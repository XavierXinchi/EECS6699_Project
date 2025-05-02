# Rethinking Skip-Connections: A Systematic Study of Residual Path Designs in Deep Neural Networks

## Overview

This repository contains the official implementation and supplementary material for our research paper:

> **Rethinking Skip-Connections: A Systematic Study of Residual Path Designs in Deep Neural Networks**
>
> Di Wang, Xinchi Shi, Yufeng Gao
> Columbia University

## Abstract

Skip-connections are essential components of modern deep neural networks, significantly enhancing the training of deep architectures by facilitating gradient flow. Despite the widespread adoption of additive skip-connections, alternative designs—including gated, concatenative, and nonlinear variants—have emerged. Our work systematically compares these different skip-connection strategies under a unified experimental setup on the CIFAR-10 dataset, providing insights into their effects on optimization dynamics, generalization capability, and learned representations. We find gated and learned-scalar connections outperform the traditional additive skip, while networks without skip-connections experience substantial performance degradation.

## Key Contributions

- Comprehensive empirical evaluation of multiple skip-connection variants under a uniform training protocol.
- Detailed analyses of optimization behavior, generalization properties, and feature representations using visualization techniques such as t-SNE.
- Depth ablation studies highlighting the critical role skip-connections play in deep neural network scalability.
- Practical guidelines for selecting optimal skip-connection architectures based on application-specific requirements.

## Setup Instructions

### Requirements

- Python 3.x
- PyTorch (latest recommended)
- torchvision
- numpy
- matplotlib
- scikit-learn

### Installation

Clone the repository and install required dependencies:

```
git clone https://github.com/your-repository-link.git
cd your-repository-name
```

### Running Experiments

Navigate to the `eecs6699_code.ipynb` file and run it.

You can use various skip types (`gated`, `additive`, `learned_scalar`, `concatenative`, `relu_skip`, `droppath`, `zeroskip`, `mlp`) to replicate our experiments.

### Results

The following image is the test accuracy of our experiments. You can check `img` file for more detailed results. 

![](/img/test_accuracy.jpg)

## License

This project is licensed under the MIT License. See LICENSE for more details.