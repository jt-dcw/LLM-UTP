# A Scalable and Generic Framework for City-wide Traffic Prediction with Large Language Models  

## Introduction  
This repository provides the implementation of **LLM-UTP**, proposed in the paper *“A Scalable and Generic Framework for City-wide Traffic Prediction with Large Language Models.”*  
UTP-LLM is a novel traffic prediction framework designed to model heterogeneous traffic patterns across different datasets and urban scenarios, enabling scalable and generalizable forecasting for various transportation modes.  

---

## Project Structure  

```
LLM-UTP
├── checkpoint/          # Saved model checkpoints for training or fine-tuning
│  ├─03/   (checkpoint for PEMS03 dataset)
│  ├─04/   (checkpoint for PEMS04 dataset)
│  ├─08/   (checkpoint for PEMS08 dataset)
│  ├─bike/ (checkpoint for bike-sharing dataset)
│  ├─bj/   (checkpoint for Beijing Metro dataset)
│  ├─bus/  (checkpoint for bus dataset)
│  ├─hsr/  (checkpoint for high-speed railway dataset)
│  ├─hz/   (checkpoint for Hangzhou Metro dataset)
│  ├─nn/   (checkpoint for Nanjing Metro dataset)
│  └─taxi/ (checkpoint for taxi dataset)
├── data/                # Dataset directory
├── mode/                # Model architecture and related code
├── utils/               # Utility functions
├── .gitattributes       # Git configuration file
├── fine-tuning.py       # Script for fine-tuning models
├── main_run.py          # Main entry point for training and evaluation
├── prediction.py        # Script for inference / prediction
└── README.md            # Project description
```
---

# Prediction
In the `prediction.py` file, update the `datac` variable to the target dataset parameter and load the corresponding checkpoint. After that, simply run the script to perform prediction.
---


## Requirements  

```
torch==2.0.0
torchvision==0.15.0
transformers==4.35.0
numpy==1.24.0
scipy==1.10.0
tqdm==4.65.0
pandas==2.0.0
matplotlib==3.7.0
```

---

## System Requirements  

- **Operating System**: Windows 10  
- **CPU**: Intel i9-10900X @ 3.70GHz  
- **Memory**: 32GB RAM  
- **GPU**: NVIDIA RTX 3080 (10GB VRAM)  

---

## Contact  

- **Name**: Congwang Deng  
- **Email**: 24125724@bjtu.edu.cn  



