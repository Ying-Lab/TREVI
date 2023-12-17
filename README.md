Introduction
-----
TREVI (Transcriptional REgulation-driven Variational Inference model) is an innovative Bayesian model for multi-omics data that incorporates priori knowledge of the gene regulation process into generation process, and the causal relationship of gene regulation into the inference process.

https://github.com/Ying-Lab/Trevi

Trevi is generated by Python 3.8 and the R 4.2.1 is used during preprocessing


Installation
-----
1.Install pytorch according to your computational platform

2.Install Trevi
```bash

git clone https://github.com/Ying-Lab/Trevi

cd Trevi

pip install -r requirements.txt 
```

Running
-----
refer to demo in [a549 demo.ipynb](https://github.com/Ying-Lab/TREVI/blob/46201a7823887830b45a64c794123e7403863146/a549%20demo.ipynb)

Parameters
-----
input: the count matrixs(numpy) of gene counts, gene accessibility score, cell label, TF-target gene reference

output: trained model 

-----
other parameters:

learning_rate : learning rate for Adam optimizer, default 1e-3.

decay_rate : decay rate for Adam optimizer, default 0.97.

beta_1 : beta-1 parameter for Adam optimizer, default 0.99.

cuda : use GPU(s) to speed up training, default True.

float64 : use double float precision, default False.

config_enum : parallel, sequential or none. uses parallel enumeration by defaultdefault "parallel".

num_epochs : number of epochs to run, default 50.

decay_epochs : decay learning rate every #epochs, default 20.

batch_size : number of images (and labels) to be considered in a batch ,default 60.

External links
-----
Trevi along with detailed documentation is freely accessible at [https://trevi.readthedocs.io/en/master/](https://trevi.readthedocs.io/en/master/) under the MIT License.




