# Pytorch Geometric Temporal Example Models
This repository in intended for simple illustrative examples on how the layers implemented in <br />
*PyTorch Geometric Temporal* can be used or showcase the shortcomings of some of the PyG-T implementations.

### Origin & Purpose
The official examples given on https://pytorch-geometric-temporal.readthedocs.io/en/latest/modules/root.html <br />
and described in the accompanying paper https://arxiv.org/abs/2104.07788 contain technical errors making the
models unable to learn.

### Data
All models are evaluated on the *Hungarian Chicken Pox* time series dataset provided in the library. <br />
The dataset is traversed with a sliding window of stride 1.

### Model Training
Recurrent models are trained on 20% of the training data in a sequential manner, <br />
while attention based models are trained on 40% of the data that is shuffled and batched. <br />
Learning rate and number of epochs vary depending on model complexity.
