# DiffBCE
This is a Python implementation of `DiffBCE: Difference Contrastive Learning for Binary Code Embeddings` .


## Dependencies
- Python >= 3.8
- angr >= 9.2.32
- angr-utils >= 0.5.0
- torch >= 1.7.1

## Installation
Describe how to install the project and all dependencies.
```bash
git clone https://github.com/your-username/project-name.git
cd project-name
pip install -r requirements.txt
```

## Usage
This project consists of two main steps: preprocessing the binary file, and then training the encoder for instruction sequence using DiffBCE. Below are the details on how to run each step:

### Dataset
please download form https://drive.google.com/drive/folders/1FXlrGiZkch9bnAxlrm43IhYGC3r5NveA

### Preprocessing

The preprocessing step involves generating features from the binary data. You can use the `feature_generator.py` script located in the `./src/preprocess/` directory for this purpose.

```bash
cd src
python preprocessing.py
```

### DiffBCE Training

Once preprocessing is complete, you can proceed to train the model using the NFSR algorithm. Use the `train.py` script located in the ./src/ directory for this step.

```bash
python train.py
```
Make sure you have navigated to the appropriate directories before running these commands. Modify any parameters in the scripts as needed to suit your specific requirements.
