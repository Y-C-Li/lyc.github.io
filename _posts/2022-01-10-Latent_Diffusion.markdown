---
layout: single
title:  "Latent Diffusion"
date:   2022-01-10 10:12:48 +0800
categories: CompVis 计算机视觉 Codes
---
Public Source: Forked from [Here](https://github.com/CompVis/latent-diffusion)

First, prepare your environment:

Open your file and change the directory of `latent-diffusion` file

```shell
conda env create -f environment.yaml
conda activate ldm
```

For me, there is an error message like this:

```bash
CommandNotFoundError: Your shell has not been properly configured to use 'conda activate'.
If using 'conda activate' from a batch script, change your
invocation to 'CALL conda.bat activate'.
```

There may be problems about `conda activate`, do this:

```bash
source activate
source deactivate
# Then, try conda activate again
conda activate ldm
```

Then run the following script downloads und extracts all available pretrained autoencoding models.

```bash
bash scripts/download_first_stages.sh
```

But it appears that I don't have a `wget` package

So first download the `wget` package here.