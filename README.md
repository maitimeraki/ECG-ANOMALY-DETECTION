# ECG Anomaly Detection

## Overview
This repository contains code and resources for detecting anomalies in ECG (electrocardiogram) signals using LSTM (Long Short-Term Memory) networks, monitored with MLflow for effective tracking of experiments, models, and metrics. 

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Data Preprocessing](#data-preprocessing)
- [Model Architecture](#model-architecture)
- [Training the Model](#training-the-model)
- [MLflow Monitoring](#mlflow-monitoring)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction
ECG anomaly detection is crucial in identifying irregular heartbeats and other cardiac conditions. This project utilizes LSTM networks, designed for sequential data, to capture temporal dependencies in ECG signals.

## Installation
To replicate this project, begin with cloning the repository:

```bash
git clone https://github.com/maitimeraki/ECG-ANOMALY-DETECTION.git
cd ECG-ANOMALY-DETECTION
```

Ensure you have Python installed (preferably version 3.7 or newer) and install the required packages:

```bash
pip install -r requirements.txt
```

## Data Preprocessing
The data should be preprocessed to ensure it is suitable for training the LSTM model. This includes normalization, segmentation, and any additional transformations necessary for improving model performance.

## Model Architecture
The model comprises layers tailored for processing time-series data:
- Input Layer
- LSTM Layers (for capturing sequential patterns)
- Dense Layer (for classification)

## Training the Model
Training can be initiated using the following command:

```bash
python train_model.py
```

This script will also log parameters and metrics to MLflow for tracking purposes.

## MLflow Monitoring
To start the MLflow server and visualize the experiments in your browser, run:

```bash
mlflow ui
```

Head to `http://127.0.0.1:5000` to see the logged metrics and experiment results.

## Usage
After training your model, you can use it to detect anomalies in new ECG data. The inference can be done via:

```bash
python predict.py --data path_to_data
```

## Contributing
Contributions are welcome! Please submit a pull request or open an issue to discuss your ideas.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Contact
For any inquiries regarding this project, feel free to contact the maintainer at maitimeraki@example.com.