# Building a CI/CD Pipeline with Azure
 
## Project Overview
In this project, a complete CI/CD pipeline is built using GitHub and Microsoft Azure.  
The project demonstrates core DevOps principles by implementing Continuous Integration (CI) using GitHub Actions and Continuous Delivery (CD) using Azure Pipelines and Azure App Service.
 
The repository contains a Python-based machine learning application built with Flask. The CI pipeline performs linting, testing, and dependency installation, while the CD pipeline deploys the application to Azure App Service.

 ## Architecture Diagram
 
The following diagram illustrates the overall architecture and workflow of the project, including source control, CI/CD pipelines, and deployment to Azure App Service.
 
![Architecture Diagram](./screenshots/Architecture.png)
 
**Architecture Flow:**
- Source code is managed in GitHub
- GitHub Actions performs Continuous Integration (linting and testing)
- Azure Pipelines enables Continuous Delivery
- The application is deployed to Azure App Service (PaaS)
- A Flask-based Machine Learning API serves predictions
 
---

## Instructions for Running the Python Project
 
### Prerequisites
Ensure the following tools are installed on your system:
 
- Python 3.8 or higher
- Git
- Make
- Azure CLI (for deployment-related steps)
- An active Azure subscription

### Step 1: Clone the Repository
```bash
git clone https://github.com/<your-username>/<your-repository-name>.git
cd <your-repository-name>

### Step 2: Create and Activate a Virtual Environment
Create a Python virtual environment to isolate project dependencies.
 
```bash
python -m venv venv
source venv/bin/activate   # Linux / Mac
venv\Scripts\activate      # Windows


### Step 3: Install Dependencies
Install all required Python packages needed to run the application.
 
```bash
make install


### Step 4: Run Lint Checks
Run linting to analyze the Python code for style issues and best practices.
 
```bash
make lint

### Step 5: Run Unit Tests
Run automated unit tests to ensure the application functions correctly.
 
```bash
make test

## Screenshots Demonstrating Key Steps
 
### 1. Successful Linting and Testing in Azure Cloud Shell
This screenshot shows the project running in Azure Cloud Shell with successful execution of both lint checks and unit tests using the Makefile.
 
![Cloud Shell Lint and Test Success](./screenshots/Test_Success.png)
 
---
 
### 2. Successful Continuous Integration Using GitHub Actions
This screenshot demonstrates a successful GitHub Actions pipeline run, confirming that Continuous Integration is working correctly with automated linting and testing.
 
![GitHub Actions Build Success](./screenshots/GitPipeline_build.png)
 
---
 
### 3. Successful Deployment Using Azure Pipelines
This screenshot shows a successful Azure Pipeline execution, confirming Continuous Delivery and deployment of the application to Azure services.
 
![Azure Pipeline Build Success](./screenshots/AzurePipeline_build.png)
