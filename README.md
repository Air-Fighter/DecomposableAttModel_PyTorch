# DecomposableAttModel_PyTorch

Rebuild the model in paper [A Decomposable Attention Model for Natural Language Inference](https://arxiv.org/pdf/1606.01933.pdf).
However, the activation function has been changed to SELU and the optimizing algrithm is Adadelta.

The project is based on the [snli example project from PyTorch](https://github.com/pytorch/examples/tree/master/snli).

## Requirements
1. PyTorch
2. torchtext

## Setup before running
1. change the following arguments of SNLI and GLOVE in **utils.py** to yours:
```
parser.add_argument('--snli_root', type=str, default='/data/shawnguo/')
parser.add_argument('--data_cache', type=str, default=os.path.join('/data/shawnguo/', 'GloVe'))
parser.add_argument('--vector_cache', type=str, default=os.path.join('/data/shawnguo/', 'GloVe/input_vectors.pt'))
```
2. run **train.py** 
