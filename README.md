This repo forks the Meta Research SAM3 repo for Viral Plaque image segmentation. <br>
The default prompt is ```spot```; change it if you want to try other words.

⚠️ Before using SAM 3, please request access to the checkpoints on the [SAM 3 Hugging Face repo](https://huggingface.co/facebook/sam3).
Once accepted, you need to be authenticated to download the checkpoints. You can do this by running the following steps in the command terminal of your device.<br> (e.g. ```hf auth login``` inside your terminal after generating an access token in your huggingface profile settings.) <br>The Access Token only needs access to the sam3 repo.

**Installation:**
**Prerequisites**<br>
- [Python 3.12 or higher](https://www.python.org/downloads/)
- [PyTorch 2.7 or higher](https://pytorch.org/get-started/locally/): ```pip install torch torchvision --index-url https://download.pytorch.org/whl/cu128``` 
- CUDA-compatible GPU with CUDA 12.6 or higher
- [CUDA Toolkit installed on your local device](https://developer.nvidia.com/cuda-downloads)
- [Anaconda](https://www.anaconda.com/download/) (Miniconda is sufficient)

**Create a new Conda environment**:<br>
Open Anaconda Prompt
```conda create -n sam3 python=3.12```
```conda deactivate```
```conda activate sam3```

**Clone the repository and install the package**:<br>
```git clone https://github.com/rayhouhou/sam3.git``` <br>
```cd sam3``` <br>
```pip install -e``` . <br>
Install additional dependencies for notebooks:
```pip install -e ".[notebooks]"``` <br>

**Still in your Anaconda Prompt Terminal, open the notebook** <br>
```jupyter notebook examples/sam3_image_predictor_example.ipynb``` <br>

**Add plates to be analysed to the following folder**:
```sam3\assets\images\plaques```
**Example Output**
<img width="896" height="776" alt="image" src="https://github.com/user-attachments/assets/d21b64dd-df1e-488a-8e07-32617c67938a" />

