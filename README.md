Towards Next-Generation Hybrid Quantum Convolutional Neural Networks: A Systematic Architecture
This repository contains the research and findings from our paper, "Towards Next-Generation Hybrid Quantum Convolutional Neural Networks: A Systematic Architecture." We explore a framework for designing robust, next-generation hybrid quantum-classical machine learning models optimized for the Noisy Intermediate-Scale Quantum (NISQ) era.

📜 Abstract
Quantum Convolutional Neural Networks (QCNNs) offer a powerful quantum-native framework for machine learning, leveraging high-dimensional Hilbert spaces and quantum parallelism to overcome the limitations of classical models. This work proposes a systematic approach to designing hybrid QCNN (HQCNN) architectures that enhance expressive power while accommodating the constraints of current NISQ hardware. We introduce and benchmark several novel quantum-classical constructs, demonstrating significant performance gains through the strategic combination of quantum circuits and classical deep learning techniques. Our findings on challenging tasks in medical imaging and quantum phase recognition highlight improved classification accuracy, parameter efficiency, and noise robustness, paving the way for practical quantum machine learning applications.

✨ Key Features & Architectures
This research introduces and evaluates a suite of novel HQCNN architectures designed to push the boundaries of near-term quantum machine learning.

🧠 Deep MERA QCNN: An architecture inspired by the Multiscale Entanglement Renormalization Ansatz (MERA) from condensed matter physics, providing a hierarchical structure that is naturally robust against the barren plateau problem.

🔧 Hardware-Efficient Ansatz (HEA)-QCNN: A pragmatic design that prioritizes compatibility with the limited connectivity and gate sets of current NISQ devices, ensuring near-term viability.

🌿 Branching QCNN (bQCNN): An expressive model that utilizes mid-circuit measurements to enable dynamic, data-dependent computational paths, effectively creating an ensemble of quantum models within a single circuit.

📐 Equivariant QCNN (EQCNN): A sophisticated architecture that integrates geometric symmetries directly into the model, enforcing an inductive bias that improves generalization and parameter efficiency for structured data.

🧪 Experimental Analysis & Results
We conducted extensive classical simulations to benchmark our proposed models against classical baselines and simpler quantum models.

Datasets
Classical Imaging: MNIST, Fashion-MNIST

Medical Imaging: Medical MNIST, Breast Cancer Diagnostics, Brain Tumor MRI

Quantum-Native Data: Transverse-Field Ising (TFI) and XXZ model ground states for quantum phase recognition.

Key Findings
Synergistic Advantage: HQCNN models consistently outperformed both their standalone classical and quantum components, demonstrating a true synergistic benefit.

Superior Performance: The proposed architectures, particularly the bQCNN, achieved state-of-the-art accuracy on benchmark tasks like MNIST classification.

Noise Robustness: Through the use of error mitigation techniques like Zero-Noise Extrapolation (ZNE) and AdaBoost, our hybrid models showed significantly improved resilience to simulated hardware noise.

Parameter Efficiency: Architectures like the EQCNN achieve high accuracy with a remarkably small number of trainable parameters, a critical feature for near-term quantum hardware.

Quantum-Native Advantage: On quantum phase recognition tasks, our quantum models substantially outperformed all classical baselines, highlighting a clear advantage for problems with underlying quantum structure.

🚀 Getting Started
(This section is a placeholder for when code is added to the repository.)

Prerequisites
pip install qiskit scikit-learn pytorch

Installation
Clone the repository:

git clone https://github.com/your-username/HQCNN.git

Navigate to the project directory:

cd HQCNN

Running an Experiment
python train.py --model bqcnn --dataset mnist --epochs 50

📄 Citation
If you use this research in your work, please cite our paper:

@article{your_team_2025_hqcnn,
  title={Towards Next-Generation Hybrid Quantum Convolutional Neural Networks: A Systematic Architecture},
  author={Author 1 and Author 2 and Author 3},
  journal={Journal of Quantum Information},
  year={2025},
  volume={XX},
  pages={XXX-XXX}
}

📜 License
This project is licensed under the MIT License - see the LICENSE.md file for details.
