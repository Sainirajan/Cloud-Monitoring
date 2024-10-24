# Cloud Monitoring Application

## Overview

This Cloud Monitoring Application is built using Flask and leverages the `psutil` library to monitor CPU and memory usage. The application provides a web interface that displays real-time metrics and alerts users when resource usage exceeds specified thresholds.

## Features

- Displays current CPU and memory usage.
- Alerts when CPU or memory usage exceeds 80%.
- Built with Flask, providing a simple web interface.

## Prerequisites

- Python 3.9 or higher
- Docker (for containerization)

## Installation

1. Clone the repository:
   git clone https://github.com/Sainirajan/Cloud-Monitoring.git
   cd Cloud-Monitoring

2. Install dependencies:
   pip install -r requirements.txt

## Usage

To run the application locally:

1. Set the FLASK environment variable:
   export FLASK_APP=app.py

2. Run the Flask application:
   flask run --host=0.0.0.0

The application will be accessible at `http://localhost:5000`.

## Docker Setup

To run the application in a Docker container:

1. Build the Docker image:
   docker build -t cloud-monitoring .

2. Run the Docker container:
   docker run -d -p 5000:5000 cloud-monitoring

Access the application at `http://localhost:5000`.

## License

This project is licensed under the MIT License.
