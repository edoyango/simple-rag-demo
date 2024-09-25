# simple-rag-demo
Showing how easy it is to get started with LLMs and RAGs!

The instructions are assuming setup on Milton.

This requires at least 11GB GPU RAM and 4GB host RAM.
If running on CPU only, available RAM needs to be at least 16GB.

The demo is in `demo.ipynb` and is fairly barebones.

## Setup

Get the repo

```bash
git clone https://github.com/edoyango/simple-rag-demo.git
cd simple-rag-demo
```

Setup the environment.

```bash
module load micromamba
ENV_PATH=/vast/scratch/users/$USER/rag-env
micromamba create -p $ENV_PATH -f env.yml
micromamba activate $ENV_PATH
```

Register the environment for use with Jupyter.

```bash
python -m ipykernel install --user --name rag-demo --display-name "Python (rag-demo)"
```

I recommend you open the notebook in a P100 GPU Jupyter session requestion around 8GB RAM.

