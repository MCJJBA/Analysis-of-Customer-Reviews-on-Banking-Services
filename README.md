# Moroccan Bank Reviews Analysis

> 🏦 Advanced ETL pipeline for analyzing customer reviews of bank agencies across Morocco using Google Maps data and ML-powered sentiment analysis.

[![Python 3.11](https://img.shields.io/badge/Python-3.11-blue.svg)](https://www.python.org/downloads/)
[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-14+-blue.svg)](https://www.postgresql.org/)

## 🎯 Project Overview

This project analyzes customer sentiment towards Moroccan banks by processing Google Maps reviews through an automated ETL pipeline, focusing on the Daraa-Tafilelt region.

### Key Features

- 🤖 Automated Google Maps review extraction
- 🔍 ML-powered multilingual sentiment analysis
- 📊 Interactive dashboards and visualizations
- 🗃️ PostgreSQL database integration
- 🔄 Automated data pipeline with Airflow

## 🚀 Quick Start

```bash
# Clone the repository
git clone https://github.com/yourusername/Bank-Reviews-Morocco.git
cd Bank-Reviews-Morocco

# Create virtual environment
python -m venv env
source env/bin/activate

# Install dependencies
pip install -r requirements.txt

# Set up environment variables
cp .env.example .env
# Edit .env with your credentials
```

Installation and Initialization of Airflow

This guide explains how to install Apache Airflow and initialize it on Linux and Windows systems. It also describes the recommended organization for your DAGs files.
1. Prerequisites

    Python 3.7 or higher must be installed on your machine.
    It is recommended to use a virtual environment (venv or conda).

2. Installing Airflow
For Linux
bash

# Create and activate a virtual environment (optional but recommended)
python3 -m venv venv
source venv/bin/activate

# Install Apache Airflow via pip
pip install apache-airflow

For Windows
cmd

REM Create and activate a virtual environment (optional but recommended)
python -m venv venv
venv\Scripts\activate

REM Install Apache Airflow via pip
pip install apache-airflow

3. Initializing Airflow

After installation, initialize Airflow's database:
bash

airflow db init

4. Creating the dags Folder

Airflow looks for workflow files (DAGs) in a folder called dags.

    Create a folder named dags at the root of your project or in your preferred location:
    bash

mkdir dags

Place your DAG Python files in this folder.

    For example, put your Airflow scripts (my_dag.py, etc.) inside the dags folder.

Configure Airflow to point to this folder (optional if you use the default structure):

    Edit the airflow.cfg file (dags_folder variable) or set the environment variable:
    bash

        export AIRFLOW__CORE__DAGS_FOLDER=$(pwd)/dags

5. Starting the Webserver and Scheduler

In two separate terminals, run:
bash

# Start the webserver
airflow webserver

# Start the scheduler
airflow scheduler

Access the Airflow interface at http://localhost:8080.
Summary

    Install Airflow with pip in a virtual environment.
    Initialize Airflow using airflow db init.
    Create a dags folder to store your Airflow workflows.
    Place your DAG files in that folder.
    Start the webserver and scheduler to use Airflow.



## 🛠️ Technology Stack

- **Data Collection**: Google Maps API
- **Processing**: Python
- **ML/NLP**: Transformers
- **Storage**: PostgreSQL
- **Orchestration**: Apache Airflow
- **Visualization**: Looker studio

## 📊 Visualizations & Dashboard

Access our interactive dashboard: [Bank Reviews Dashboard](https://lookerstudio.google.com/reporting/a391b1ac-d8ac-4d24-8773-7ec4c162b78a)

The dashboard includes:
- Real-time sentiment analysis results
- Bank performance comparisons
- Regional distribution of reviews
- Customer satisfaction trends
- Topic analysis by bank and region
- Review volume patterns

Key visualizations include:
- Sentiment distribution by bank
- Regional satisfaction map
- Topic modeling insights
- Trend analysis over time
- Review volume by location
- Rating distributions


## 📝 License

This project is MIT licensed. See [LICENSE](LICENSE) for details.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📫 Contact

[@IzeriaAbdellatif](https://github.com/yourusername) , [@MedTahiri](https://github.com/MedTahiri)

Project Link: [https://github.com/yourusername/Bank-Reviews-Morocco](https://github.com/yourusername/Bank-Reviews-Morocco)
