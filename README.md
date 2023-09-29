# pFGD
pFGD - Defending Against Gradient Inversion Attacks

In this work, we explore the implications of Gradient Inversion attacks in FL and propose a novel defence mechanism, called Pruned Frequency-based Gradient Defence (pFGD), to mitigate these risks. Our defence strategy combines frequency transformation using techniques such as Discrete Cosine Transform (DCT) and employs pruning on the gradients to enhance privacy preservation.

## Experiment Setup
Change the following variables as needed.

```
dataset = 'MNIST'
PRUNING_PERCENTAGE = 0.01
Iteration = 100
num_exp = 1
```

```shell
python3 experiments.py
```