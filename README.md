## pFGD: Mitigating Gradient Inversion Attacks in Federated Learning with Frequency Transformation

This work is published at the **SECAI: ESORICS 2023 International Workshop, Lecture Notes in Computer Science (LNCS,volume 14399) [Mitigating Gradient Inversion Attacks in Federated Learning with Frequency Transformation](https://doi.org/10.1007/978-3-031-54129-2_44)**

Bibtext
```
@inproceedings{palihawadana2023mitigating,
  title={Mitigating Gradient Inversion Attacks in Federated Learning with Frequency Transformation},
  author={Palihawadana, Chamath and Wiratunga, Nirmalie and Kalutarage, Harsha and Wijekoon, Anjana},
  booktitle={European Symposium on Research in Computer Security},
  pages={750--760},
  year={2023},
  organization={Springer}
}
```


In this work, we explore the implications of Gradient Inversion attacks in FL and propose a novel defence mechanism, called Pruned Frequency-based Gradient Defence (pFGD), to mitigate these risks. Our defence strategy combines frequency transformation using techniques such as Discrete Cosine Transform (DCT) and employs pruning on the gradients to enhance privacy preservation.

Pruned frequency gradients prevents model inversion through adding noise and parameter reduction.

![image](https://github.com/chamathpali/pFGD/assets/5123109/b8807ee8-74f1-4e32-b1e5-2c4a9bd307a1)


This work is published at the Workshop on Security and Artificial Intelligence (SECAI) 2023 In conjunction with ESORICS 2023

## Experiment Setup

We have adapted the experiment setup from [iDLG](https://github.com/PatrickZH/Improved-Deep-Leakage-from-Gradients)

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

### Experiment Variaions

- Vanilla (original method without modifications)
- Vanilla with pruning (pruning applied to the vanilla method)
- DCT (applying only DCT transformation) 
- DCT with pruning (pruning applied to the DCT transformed gradients)

All experiments are perfomed on 100 attack iterations each 1,000 experiments (random initialised)


### Results

Pruning Percentages
- [1% Pruning](https://github.com/chamathpali/pFGD/blob/main/Results-MNIST-p-0.01.pdf)
- [0.1% Pruning](https://github.com/chamathpali/pFGD/blob/main/Results-MNIST-p-0.001.pdf)




