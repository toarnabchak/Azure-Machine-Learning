# Chapter-1 - Azure Machine Learning: the Overview

![image](https://github.com/user-attachments/assets/6365a41b-b3fd-47d3-9e16-6d10cd136121)

---

### Introduction to Azure Machine Learning
- The section is part of a multi-part series on Azure Machine Learning, presented by Kevin Feasel, a consultant specializing in data platforms.
- This series will cover:
  - Basics of Azure Machine Learning
  - Automated machine learning
  - Using the Azure ML Designer
  - Writing code with the Python SDK
  - Implementing MLOps (machine learning operations) with GitHub actions
- The content will supplement Kevin’s presentations on Azure ML.

---

### Core Concepts of Azure Machine Learning

#### Architecture Diagram and Key Components
- **Azure ML Workspace**: The central core and interaction hub for ML components, accessed through Azure ML Studio or other interfaces.
- **Additional Services**:
  - **Azure Storage Account**: For storing data in blob storage containers and file shares.
  - **Azure Container Registry**: Hosts Docker containers for model deployment, helping to manage versioning and isolation.
  - **Azure Key Vault**: Stores sensitive information like database connection strings and tokens securely.
  - **Azure Application Insights**: Tracks and stores application logs.

#### Compute Resources
- **Compute Instances**: Virtual machines dedicated to individual data scientists, treated as ephemeral resources.
- **Compute Clusters**: Groups of machines for large-scale model training. They auto-shut down when idle to reduce costs, making them efficient for high-demand computational needs.

#### Linked Services and Datastores
- **Datastores**: Services hosting data, with seven types of Datastores (Azure services).
- **Compute Targets**: Five compute targets, including Spark-based services like Databricks and Azure Synapse Analytics.

---

### Assets in Azure Machine Learning

#### Datasets and Training Pipelines
- **Datasets**: Collections of data for model training.
- **Training Pipeline**: Used to test different algorithms and processes in an experiment.

#### Inference Pipelines and Endpoints
- **Inference Pipeline**: Allows other services to make predictions using new data through an endpoint.
- **REST API Endpoint**: Wraps the model, enabling JSON requests and responses for real-time inference.

#### Managed Resources and Datastore Types
- **Datastores**: Hosts for data types like blob storage, file shares, and SQL databases.
- **Data Assets**: Created and stored in the workspace, for example, CSV files and binary data.

---

### Working with Azure ML Studio

#### Setting Up the Azure ML Workspace
- **Creating a New Workspace**:
  - Steps include selecting a subscription, choosing a resource group, and specifying a workspace name.
  - Additional configurations like Managed Identities and Data Encryption are available.
  
#### Accessing and Configuring Compute Instances
- **Compute Instances**:
  - Idle shutdown settings save costs.
  - Schedule-based shutdowns prevent unnecessary charges.
  
#### Data Management
- **Creating and Managing Datastores**: Limited to specific Azure types, set up by selecting “Create” and choosing relevant options.
- **Data Assets in Action**: For example, Chicago parking ticket data is used as a sample dataset.

---

### Model Training and Experimentation

#### Jobs and Pipelines
- **Experiments**: Defined tasks (e.g., using different algorithms or tuning hyperparameters).
- **Pipeline Jobs**: Multiple runs of training or inference pipelines under a single experiment.

#### Model Registry and Endpoints
- **Model Registration**: Trained models are stored and accessible through the registry.
- **Endpoints for Inference**: Real-time inference through a REST API endpoint, enabling interaction with deployed models.

#### Environments for Model Training
- **Microsoft-Curated Environments**: Includes options pre-installed with tools like TensorFlow and PyTorch.
- **Custom Environments**: Docker files with environment instructions and required Python packages.

---

### Conclusion
- This section serves as an overview, setting up for hands-on applications in later sections.
- The next section will dive into **Automated Machine Learning** within Azure ML, covering model training in-depth. 

---
