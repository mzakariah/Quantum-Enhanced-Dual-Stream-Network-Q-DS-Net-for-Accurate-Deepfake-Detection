Quantum-Enhanced-Dual-Stream-Network-Q-DS-Net-for-Accurate-Deepfake-Detection
The suggested architecture incorporates a spatial stream for fine-grained visual artifact learning and a temporal stream for motion inconsistency modeling, and quantum-enhanced convolution modules are proposed to improve the representation of weak forensic traces that traditional feature extractors may fail to capture. it gets an accuracy of 99.89 . Quantum-Enhanced Dual-Stream Network is one of the deepfake detectors, which is the primary component of the repository. In this project spatial and frequency-domain feature extraction have been taken in the form of a dual-stream structure with a complex fusion process and quantum based component to improve on discrimination.

The repository constituted contain all parts required which consist of:

* Data preprocessing pipeline
* Model architecture implementation
*Training scripts and evaluation scripts.
* Configuration settings
Commentaries and records concerning reproduction.

Installation Instructions

1. Clone the Repository

git clone <your-repository-link>
cd <repository-folder>

2.Virtual Environment
python -m venv env
In Mac.x/Linux/Mac.
env\Scripts\activate         # For Windows

3. Install Dependencies

Requirements. All the libraries are incorporated in TXT.

pip install requirements.txt.

4. Additional Requirements

Install: make sure that the following has been installed:

* Python ≥ 3.8
All the versions of the NVIDIA are compatible with the CUDA (non mandatory, graphic card acceleration).
implementation Minimally Vehicle Networks PyTorch/TF.


Preprocessing Pipeline

Preprocessing stage is used to obtain consistency of the data and improved models. It includes:

Framing of videos.
Face recognition and matching.
Image Recognition, Image normalization.
frequency-domain decomposition (2 nd stream )
Normative management of the data: (flips, rotation) Noise injection)

To run preprocessing:

python preprocessing/run_preprocessing.py

Model Architecture

1. Dual-Stream Network

Frequency Stream: The artifacted FFT/DCT logs of the inputs were made logs.

2. Fusion Mechanism

Combines both streams.
* Has attention-based weight fusion technique.
The complementary feature representation is increased.

3. Quantum Module

Feature mapping quantum-inspired.
Increases the non-locality of features space.
Helps are non linear and convoluted.

The modules are discussed at the detail.

Training Instructions

To train the model:

python training/train.py-config configs/train_config.yaml

Key Training Parameters

Object type Batch size: (configurable default: 32/64)
* Epochs: configurable (e.g., 30–50)
Learning rate: is a parameter of the config.
* Optimizer: Adam / SGD
Loss objective:auc Loss of custom / Binary Cross-Entropy.

Evaluation

The trained model can be tested to do this:

Evaluationpython analyze/ evaluate.py -modelpath savedmodel.

Metrics Used

* Accuracy
* Precision
* Recall
* F1-Score
* ROC-AUC

The scripts of the analysis give numerical and graphical plots.

Reproducibility

To ensure reproducibility:

Model Procedure: Check to ensure that configuration files have proper random seeds in them.

* Retuse identical hyperparameters.

Configuration

The experiments will be configured using configuration files the arguments of which may look as follows:

configs/train_config.yaml
configs/eval_config.yaml

You can modify:

* Dataset paths
* Model parameters
* Training hyperparameters

Notes

It has been highly suggested to accelerate the training process through the assistance of GPU.
Preparation of paths to datasets also needs to be prepared before it is neglected.
Finetuning is made available just in case of pre trained weight finetuning.

Contribution

Contributions are welcome. You can:

* Report issues
* Suggest improvements
* Submit pull requests

License

This is a research undertaking. Refer to our work in case of using this repository.

Final Remark

The repository will also aim to be a complete self-contained and reproducible repository would do obviously:

* Dual-stream architecture
* Fusion mechanism
* Quantum-inspired module
