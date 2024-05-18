# duration_prediction
This project showcases a machine learning pipeline for predicting the duration of trips, built as part of an MLOps (Machine Learning Operations) capacity building projects. The goal of this project is to demonstrate the practical application of MLOps principles in developing, deploying, and maintaining a machine learning model.

# Table of Contents
- Project Overview
- Installation
- Usage
- Project Structure
- Model Details
- Contributing
- License

# Project Overview
The Duration Prediction Project showcases a complete machine learning pipeline, from data preprocessing to model deployment and monitoring. The project emphasizes the integration of MLOps practices to ensure the reliability and scalability of the machine learning - model in a production environment.

# Installation
To run this project locally, follow these steps:

1. Clone the repository:
```
git clone https://github.com/your-username/duration-prediction-project.git
cd duration-prediction-project
```
2. Create and activate a virtual environment:
```
python -m venv venv
source venv/bin/activate
# On Windows, use `venv\Scripts\activate`
```
3. Install the required dependencies:
```
pip install -r requirements.txt
```
4. Set up Docker (if applicable):
Ensure Docker is installed and running on your system. Build the Docker image:
```
docker build -t duration-prediction .
```
# Usage
# Running the Pipeline
To run the data preprocessing and model training pipeline, use the following command:
```
python src/train_pipeline.py
```
# Deploying the Model
To deploy the model using Docker, run:
```
docker run -p 5000:5000 duration-prediction
```
The model will be accessible at `http://localhost:5000`.

# Monitoring
For monitoring the deployed model, ensure Prometheus and Grafana are configured and running. Follow the instructions in the `monitoring/` directory to set up the monitoring tools.

# Project Structure
```
duration-prediction-project/
| data/
│   ├── raw/
│   ├── processed/
├── src/
│   ├── data_preprocessing.py
│   ├── train_pipeline.py
│   ├── model.py
│   ├── evaluate.py
├── docker/
│   ├── Dockerfile
├── monitoring/
│   ├── prometheus.yml
│   ├── grafana/
├── tests/
│   ├── test_model.py
│   ├── test_preprocessing.py
├── .github/
│   ├── workflows/
│       ├── ci.yml
│       ├── cd.yml
├── requirements.txt
├── README.md
└── LICENSE
```

<!--
# Model Details
The model used for duration prediction is a [model type] trained on Green Trip Dataset. Key features include [mention key features used]. The model is evaluated using [evaluation metrics] and achieves [performance metrics].

Contributing
Contributions are welcome! Please read the CONTRIBUTING.md file for guidelines on how to contribute to this project.

License
This project is licensed under the MIT License. See the LICENSE file for details.
-->
