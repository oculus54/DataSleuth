# DataSleuth

### Multi-Agent AI Data Analyst using CrewAI

## Overview

DataSleuth is an AI-powered data analysis application that uses specialized CrewAI agents to analyze CSV datasets, identify data-quality issues, detect anomalies, generate visualizations, and produce automated reports.

Users upload a CSV file and receive a structured analysis of their data through a simple Streamlit interface.

## Tech Stack

* **Python**: Core programming language
* **CrewAI**: Multi-agent orchestration
* **Pandas & NumPy**: Data processing and cleaning
* **Scikit-learn**: Anomaly detection
* **Matplotlib & Seaborn**: Data visualization
* **Streamlit**: Web interface
* **Ollama**: Optional local LLM inference

## Agent Architecture

1. **Data Profiler:** Examines dataset structure, column types, missing values, and duplicates.
2. **Data Cleaner:** Recommends and applies approved cleaning operations.
3. **Statistical Analyst:** Calculates descriptive statistics and identifies relationships between variables.
4. **Anomaly Detector:** Identifies unusual observations using statistical methods and machine learning.
5. **Report Generator:** Summarizes findings and generates a report with charts and evidence.

## Workflow

```text
CSV Upload
    |
    v
Data Profiling
    |
    v
Data Quality Inspection
    |
    v
Data Cleaning
    |
    v
Statistical Analysis
    |
    v
Anomaly Detection
    |
    v
Visualization
    |
    v
Automated Report
```

CrewAI coordinates the agents, while Python libraries perform the actual calculations to ensure numerical results are reproducible.

## Core Features

* CSV dataset upload and preview
* Automatic dataset profiling
* Missing-value and duplicate detection
* Data cleaning with an operation log
* Descriptive statistics and correlation analysis
* Statistical and ML-based anomaly detection
* Automatic chart generation
* AI-generated analysis summaries
* Downloadable cleaned CSV and HTML report

## Project Structure

```text
DataSleuth/
├── app.py
├── agents.py
├── tasks.py
├── tools.py
├── requirements.txt
├── README.md
├── sample_data/
│   └── dataset.csv
└── outputs/
    ├── charts/
    ├── cleaned_data.csv
    └── report.html
```

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/DataSleuth.git
cd DataSleuth
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

Activate it:

**Windows**

```bash
.venv\Scripts\activate
```

**Linux / macOS**

```bash
source .venv/bin/activate
```

### 3. Install dependencies

```bash
pip install crewai streamlit pandas numpy scikit-learn matplotlib seaborn
```

Add any additional dependencies required by the selected LLM integration.

### 4. Run the application

```bash
streamlit run app.py
```

## Future Improvements

* Support Excel and JSON datasets
* Add interactive visualizations
* Introduce natural-language questions about datasets
* Add downloadable PDF reports
* Support larger datasets with background processing

## Project Goal

Build a practical multi-agent AI system that combines LLM-based reasoning with reliable data-processing tools to automate exploratory data analysis.

**Note:** This repository describes the intended architecture. Features should only be marked as implemented after their corresponding code and tests are complete.
