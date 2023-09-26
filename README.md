# Weights and Biases Tutorial on HiperGator
>This Requires a Weights and Biases Account (https://wandb.ai/site)

## HiPerGator Open On-Demand
1. Navigate to the Open On-Demand Website ([ood.rc.ufl.edu](ood.rc.ufl.edu))
2. Open a Jupyter Notebook Sesion 

## Weights and Biases Setup
1. Once you login, navigate to: https://wandb.ai/settings
2. Select, Danger Zone -> API Keys -> New Key

## Installation
1. Begin by cloning this repository to your chosen directory `\path\to\directory\`:

```
cd \path\to\directory\
git clone https://github.com/aa14av/wandb-tutorial.git
cd wandb-tutorial
```

2. Once the repository is cloned, open `example.ipynb` and select the kernel `Tensorflow-2.7.0`
   
3. Copy/paste this API Key you generated earlier into `example.ipynb` after you run the line:
   
```python
print("TensorFlow Version:", tf.__version__)
wb.login(); 
```
(It will ask for your API key) 

