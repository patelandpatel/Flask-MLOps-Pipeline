# Flask MLOps Pipeline

A lightweight Flask application designed for deploying and managing machine learning models in production environments using MLOps best practices. This project integrates Flask with essential MLOps components, including CI/CD automation, model versioning, monitoring, and logging, to ensure scalable and reliable ML deployments.

## Features

- **Model Serving**: Real-time model inference via a REST API built on Flask.
- **Automated CI/CD**: GitHub Actions for automated testing, Docker containerization, and deployment workflows.
- **Monitoring and Logging**: Integrated with Prometheus and Grafana to track performance metrics, latency, and data drift.
- **Version Control and Experiment Tracking**: MLflow integration for model tracking, version control, and reproducibility.

## Getting Started

### Prerequisites

- Python 3.8 or above
- Docker (for containerization)
- Prometheus and Grafana (for monitoring)
- Git (for version control)

### Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/patelandpatel/Flask-MLOps-Pipeline.git
   cd Flask-MLOps-Pipeline
   ```

2. **Create a Virtual Environment**:
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

### Running the Application

1. **Start the Flask Server**:
   ```bash
   flask run
   ```
2. Access the API at `http://127.0.0.1:5000`.

### Docker

1. **Build the Docker Image**:
   ```bash
   docker build -t flask-mlops-pipeline .
   ```
2. **Run the Docker Container**:
   ```bash
   docker run -p 5000:5000 flask-mlops-pipeline
   ```

## Usage

- **/predict**: Endpoint for making predictions.
- **/health**: Endpoint for health checks and status monitoring.

## Contributing

1. Fork the repository.
2. Create a new branch: `git checkout -b feature-name`.
3. Commit your changes: `git commit -m 'Add some feature'`.
4. Push to the branch: `git push origin feature-name`.
5. Open a pull request.

## License

This project is licensed under the MIT License.
