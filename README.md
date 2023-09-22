# Weights and Biases Tutorial on HiperGator
>This Requires a Weights and Biases Account (https://wandb.ai/site)

## Weights and Biases Setup
1. Once you login, navigate to: https://wandb.ai/settings
2. Select, Danger Zone -> API Keys -> New Key
3. Copy this API Key into the `example.ipynb` at `wb.login(<YOUR API KEY HERE>)`

## Installation
1. Begin by cloning this repository to your chosen directory `\path\to\directory\`:

```
cd \path\to\directory\
git clone https://github.com/aa14av/wandb-tutorial.git
```
2. Once the repository is cloned, open `example.ipynb` and select the kernel `Tensorflow-2.7.0`

You will also need to install `wandb` with the line `pip install wandb` (this is included in the notebook)
