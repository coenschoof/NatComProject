# NatComProject
This repository is for the project for the course Natural Computing at Radboud University, 2022.

Authors: Coen Schoof & Denise van Baalen.

---

Comparison of Performance of Particle Swarm Optimizer
Versus Gradient-based Optimizers

Project Aim
The aim of this project was to compare the performance of PSO when used as a neural network optimizer (i.e. a method to traverse the error space to find better network weights and biases) to more common gradient-based optimizers.
To this end, different configurations of PSO and different gradient-based optimizers have been given similar computational resources to train LeNet5 on the FashionMNIST and CIFAR-10 datasets, respectively.

Files and Run Instructions
The PSO and gradient-based optimizer experiments have been run in separate Jupyter notebooks. In this repository, you will find:
- Experiment - PSO.ipynb
- Experiment - Gradient Optimizers.ipynb

To run the experiments, follow the instructions at the top of each file. This simply consists of configuring the settings as desired and running the full notebook. Each experiment will take between 60 and 65 minutes, excluding the time to load the dataset.

Near the end of each file, a line stating 'best val acc:' will give the best validation performance, the data used in the results section of the report.

The original experiments were run in Google Colab, but, given the correct imports, it should be possible to run the notebooks locally as well. If done locally, please note that the found performance may differ if the hardware is less or more powerful than what is provided by Colab, as it may execute less or more iterations or epochs in the given time.

--------------------------------------------------------------------------------------------------------------------------------------------------------

Example of a run using a gradient-optimizer (ADAM, 1 minute, FashionMNIST)
![non-PSO](https://user-images.githubusercontent.com/23215039/174317362-3cff73c5-6d1c-4599-be8e-cc1aacf212ea.png)

Example of a run using PSO as the optimizer (c1 = c2 = 1.5, w = 0.93, num_particles = 5, 1 minute, FashionMNIST)

![PSO](https://user-images.githubusercontent.com/23215039/174318617-73067461-8a97-478b-8066-1bafb6f969a8.png)
![PSO2](https://user-images.githubusercontent.com/23215039/174318673-98c83321-d405-47a7-8d99-cf6feb8add76.png)
