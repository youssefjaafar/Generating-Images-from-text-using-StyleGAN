# Generating-Images-from-text-using-StyleGAN

## Envirionment setup
After cloning this repo, enter into the folder where you cloned the repository and run the following command to create a new conda environment with all the required packages anad dependencies.
```console
conda env create -f environment.yml
```
```console
pip install clip
pip install torch
pip install torchvision
```
## StyleGAN Weights
Download the `.pt` file from [here](https://github.com/lernapparat/lernapparat/releases/download/v2019-02-01/karras2019stylegan-ffhq-1024x1024.for_g_all.pt
) and store it inside the folder of this repo with the name `karras2019stylegan-ffhq-1024x1024.for_g_all.pt`.

## Generate faces
Run the following command to generate a face with a custom prompt. In this case the prompt is "The image of a woman with blonde hair and purple eyes"
```console
python clip_generate.py --prompt "The image of a woman with blonde hair and purple eyes"
```

The results will be stored under the folder `generations` with the name of the prompt that you have entered.
