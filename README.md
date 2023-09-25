# Weights and Biases Tutorial on HiperGator
>This Requires a Weights and Biases Account (https://wandb.ai/site)

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
   
3. Copy/paste this API Key you generated earlier into the `example.ipynb` at:
   
```python
print("TensorFlow Version:", tf.__version__)
wb.login("PASTE YOUR API KEY BETWEEN THESE QUOTATIONS"); 
```
