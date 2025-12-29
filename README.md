# Thermal-Imaging-for-Sealing-Defect-Detection-in-Pharmaceutical-Bags-Using-a-Temporal-Fusion-Network
Markdown
 |
# Code

This repository contains code for data generation (MATLAB) and multiple deep learning network training experiments (Python).

## Directory Structure

- `data_generate/`: MATLAB scripts for data generation
- `network/`: Python training code for different networks / experiments
  - Each network folder contains its own `config.py` that controls paths and output settings.

## Environment

- Conda: 25.3.1
- Python: 3.7.16

Install dependencies (example):

```bash
cd network
pip install -r requirements.txt
Training
After creating and activating the virtual environment / conda environment, run train.py inside the corresponding network folder.

Examples (run from repository root):

bash
 |
python network/TMFFNet/train.py
python network/resnet/train.py
python network/MobileNetV3/train.py
python network/ViT/train.py
Some experiments are under:

network/glass_bangle_exp/
network/Leather_Defect_Classification_exp/
Example:

bash
 |
python network/glass_bangle_exp/TMFFNet/train.py
Notes
Dataset paths must be set manually in the corresponding config.py.
Output paths and results are configured in each network folder's config.py.
License
Apache-2.0. See LICENSE.
