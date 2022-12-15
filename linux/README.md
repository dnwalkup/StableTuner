
# Stable Tuner, Linux Edition
<a href='https://discord.gg/DahNECrBUZ' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://cincydiscord.com/wp-content/uploads/2019/02/CINCYDISCORDJOIN.png' border='0' alt='Join the discord :)' /></a>


### Join the Discord!

### Special thanks to https://github.com/devilismyfriend who put this together. Buy him a <a href='https://ko-fi.com/O4O5GU04F' target='_blank'>Ko-Fi</a>

** Please note that this linux version is unstable and the performance does not currently live up to DevilIsMyFriend's standards. **

Musings
* **Use Docker Image** - This is currently tested on docker image dnwalkup/cuda:116-cudnn8-devel-u2004 -- built specifically for Runpod, but may work with other cloud providers.
* **Docker Image Base** - Ubuntu 20.04, Nvidia CUDNN 8, CUDA 1.16
* **PIP Installs** - gDown, wget, ftfy, OmegaConf, tqdm, tensorboard, transfomers, triton, pillow, iPython, pycuda, ipywidgets, jupyterlab
* **APT Installs** - zip, unzip, rename, python3, python3-apt, python3-diskutils, python3-pip

## Installation
Use the Jupyter Notebook. The code is basic at the moment and doesn't support environments outside of the docker image (e.g. with xFormers).

Once you are in your cloud environment's Juypter Notebook, click "FILE > OPEN FROM URL..." Then paste in the link for the notebook:
https://github.com/dnwalkup/StableTuner/raw/main/linux/runpod-cu116.ipynb

If your new to DreamBooth / Linux:
* Zip your training images into a folder named "dataset" (.zip)
* Upload them to google drive
* Get a link that's accessable to all
* Paste the link into the variable "goog_dataset_url" in the first Juypter Notebook cell
* If you do multiple attempts (like I always do), google will probably cap your data depending on the size of your dataset, it's good to have a backup in dropbox or your own server

* The current training doesn't include support for prior preservation loss / class images

If you know what you're doing:
* In disbelief you've read this far

## Usage
If you have any questions feel free to ask in the <a href="https://discord.gg/DahNECrBUZ">Discord</a>

## Kudos
* Shivam - For the original code and inspiration - A2 License
* Diffusers - For the latest and greatest implementations - A2 License
* Everydream - For the Aspect Ratio bucketing - MIT License
* Sygil.dev - For the environment setup - GAPLV3 License
* sd_dreambooth_extension - for the bitsandbytes files and install script
* StabilityAI - For the latest and greatest models
* The whole SD community - For making this possible
