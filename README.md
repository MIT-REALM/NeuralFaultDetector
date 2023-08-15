## Introduction

FTneuralCBF is a toolbox for designing NN-based fault-tolerant control as well as fault-detection and isolation (FDI) mechanisms. For more details, please refer to the paper: (TBD)

## Installation

git clone https://github.com/kunalgarg42/NeuralFaultDetector.git

conda create --name [CONDA ENV NAME] python=3.9

conda activate [CONDA ENV NAME]

pip install -r . requirements.txt

## Training

In order to setup the learning, first create a python file for your control-affine systems in the dynamics folder (using control_affine_system_new.py) as the base file.

Then, for CBF + u learning, create a train file following the setup of [Crazyflie_train_new file](https://github.com/kunalgarg42/NeuralFaultDetector/blob/master/train/Crazyflie_train_new.py). For training FDI, use [CF_train_Gamma_Output file](https://github.com/kunalgarg42/NeuralFaultDetector/blob/master/train/CF_train_Gamma_Output.py). 

Finally, for testing the performance of FDI, you can use [CF_test_Gamma_compare_NNs_output.py](https://github.com/kunalgarg42/NeuralFaultDetector/blob/master/test/CF_test_Gamma_compare_NNs_output.py) as the base file.

