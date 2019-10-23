# deptrans

This repository contains code for a neural-network based dependency parser. The parser contains three primary transitions: shift, right-arc and left-arc. 

An oracle is implemented to predict the next transition with perfect accuracy. Given the current stack, buffer and dependencies, the neural network will predict which transition to apply next. The error in the model's prediction is compared against the oracle and backpropagated to optimize the model parameters. 

## Training

Run `python model.py` to train the network and compute predictions on test data.