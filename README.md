## Neural approximation to the stochastic differential equation

The PyTorch implementation for the paper titled "[An Efficient Data-Driven Approximation to the Stochastic Differential Equations with Non-global Lipschitz Coefficient and Multiplicative Noise.](ccc)"  by X. Qi, T. Duan, and H. Guo. 

The contribution this paper is to propose a neural approximation called "extended continuous latent process flow" for numerically solving underlying model. The principle idea of this method is to derive a variational lower bound by constructing a posterior latent process conditional on all information over the whole time interval
to maximize the log-likelihood generated by the observations, thereby providing a feasible way to approximate the considered problem. Numerical experiments are reported to demonstrate the effectiveness and generalization performance of the proposed method.



<p align="center">
<img align="middle" src="https://github.com/JHUNAI/ECLPF/blob/main/table1.png" width="1000" />
</p>

<p align="center">
<img align="middle" src="https://github.com/JHUNAI/ECLPF/blob/main/fig1.png" width="1000" />
</p>

<p align="center">
<img align="middle" src="https://github.com/JHUNAI/ECLPF/blob/main/table2.png" width="1000" />
</p>

<p align="center">
<img align="middle" src="https://github.com/JHUNAI/ECLPF/blob/main/fig2.png" width="1000" />
</p>




## Installation
This code is developed with Python3 and Pytorch. To set up an environment with the required packages, run
```
conda create -n ECLPF
conda activate masde
pip install -r requirements.txt
```

## Training and Generation
### Ginzburg-Landau Equation.
```
python eCLPF1.py
```
### Van-der-pol Equation.
```
python eCLPF1.py
```

