<h1 align='center'>Neuro Load : Mental Workload Assessment using GSR</h1> 

**Project Duration**: May 2023 - June 2023

Neuro Load is a research project that introduces a novel approach to categorizing mental workload using Galvanic Skin Response (GSR). The project focuses on leveraging advanced signal processing techniques and machine learning to assess mental workload effectively.

## Project Overview

Mental workload is a critical factor in understanding cognitive processes, particularly in environments where optimal performance is essential. This project aimed to provide a new method for categorizing mental workload through the analysis of GSR signals.

## Technologies and Techniques Explored

- **Python**: The project was implemented in Python, taking advantage of its robust libraries for signal processing and machine learning.
- **Chirp Z Transform (CZT)**: Used for frequency analysis of the GSR signals, providing high-resolution spectral analysis.
- **Continuous Wavelet Transform (CWT)**: Applied for time-frequency analysis, enabling the identification of transient features in the GSR signals.
- **Transfer Learning**: Employed to enhance the model's ability to generalize across different datasets and improve the accuracy of mental workload classification.

## Key Features

### 1. Signal Processing
- **Feature Engineering**: Extracted meaningful features from the GSR signals using CZT and CWT to capture both frequency and time-domain characteristics.
- **Data Preprocessing**: Applied various signal processing techniques to clean and normalize the GSR data before analysis.

### 2. Machine Learning
- **Model Development**: Developed models using transfer learning techniques to classify mental workload into different categories.
- **Performance Evaluation**: Assessed the models using metrics such as accuracy, precision, and recall to ensure robust performance.

### 3. Research Contribution
- **Novel Approach**: Introduced a new method for mental workload assessment that combines advanced signal processing with machine learning.
- **Potential Applications**: The findings from this research can be applied in fields like cognitive neuroscience, human-computer interaction, and occupational health.

## Installation

To set up the project on your local machine, follow these steps:

1. **Clone the repository**:
    ```sh
    git clone https://github.com/krishnaura45/NeuroLoad.git
    cd NeuroLoad
    ```

2. **Install required dependencies**:
    ```sh
    pip install -r requirements.txt
    ```

3. **Run the Jupyter Notebooks**:
    - Start by exploring the feature engineering notebook (`nl_part1_feature_engg.ipynb`).
    - Continue with the transfer learning notebook (`nlpart2_transfer_learning.ipynb`).

## Usage

1. **Feature Engineering**:
    - Load the GSR dataset.
    - Apply CWT to extract features.
    - Visualize the signal transformations.

2. **Transfer Learning**:
    - Train the model using preprocessed features.
    - Fine-tune the model using transfer learning.
    - Evaluate the model's performance on test data.

## Example

Here's a snippet to illustrate how to apply CZT on GSR data:

```python
import numpy as np
from scipy.signal import chirp, find_peaks, peak_widths

# Example GSR data
gsr_signal = np.array([your_signal_data_here])

# Apply Chirp Z Transform
czt_signal = chirp(gsr_signal, f0=0.1, f1=1.0, t1=10, method='linear')
```

## Contributing
We welcome contributions to enhance Neuro Load. Please follow these steps to contribute:
1) Fork the repository.
2) Create a new branch: git checkout -b feature/your-feature-name.
3) Make your changes and commit them: git commit -m 'Add some feature'.
4) Push to the branch: git push origin feature/your-feature-name.
5) Open a pull request.

### REFERENCES<hr>
1) https://pubmed.ncbi.nlm.nih.gov/22778631/
2) https://ieeexplore.ieee.org/document/5663259
3) https://www.researchgate.net/publication/221532890
4) https://ieee-dataport.org/open-access/maus
5) https://pub.towardsai.net/feature-scaling
6) https://www.kaggle.com/code/samsonlo/resnet-50
7) https://arxiv.org/pdf/1611.06455.pdf 
8) https://github.com/nachi-hebbar/TL-ResNet
9) https://github.com/codebasics/deep-learning-keras-tf-tutorial

