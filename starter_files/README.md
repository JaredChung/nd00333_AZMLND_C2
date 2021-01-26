# Azure MLOPS - Deployment of AUTOML model and Automation Pipeline

In this project I will testing using Azure to build a model on the Bank Marketing Dataset to predict Term Deposit uptake and then deploy this as an API within Azure.

The main Components include:

* AutoML for building model
* Deployment API Endpoint (with benchhmarking)
* Pipeline for automation


## Architectural Diagram
 ![diagram](screenshots/diagram.png)

## Key Steps

### Step 0 - Authentication

### Step 1 - Load Data

![registereddata_f](screenshots/registereddata_f.png)

![data_load_f](screenshots/data_load_f.png)

### Step 2 - Auto ML Experiment

![automlcomplete_f](screenshots/automlcomplete_f.png)

List of all model experiments run

![topmodellist_f](screenshots/topmodellist_f.png)

Top model from Automl Run

![topmodel_f](screenshots/topmodel_f.png)

### Step 3 - Deploy the Best Model

Start Deployment of model

![deployment_f](screenshots/deployment_f.png)

Model deployed

![deploymentdone_f](screenshots/deploymentdone_f.png)

### Step 4 - Enable Logging

Run logs.py file which will allow application insights to be enabled

![pythonlog_f](screenshots/pythonlog_f.png)

![applicationinsights_f](screenshots/applicationinsights_f.png)

### Step 5 - Swagger Documentation

Run serve.py and swagger.sh to provide API documentation

![swagger1_f](screenshots/swagger1_f.png)

![swagger2_f](screenshots/swagger2_f.png)

![swagger3_f](screenshots/swagger3_f.png)

### Step 6 - Consume Model Endpoints

Test the endpoint by running endpoint.py

![endpointrun_f](screenshots/endpointrun_f.png)

Benchmark the API using Apache Benchmark

![benchmark1_f](screenshots/benchmark1_f.png)

![benchmark2_f](screenshots/benchmark2_f.png)

### Step 7 - Create and Publish a Pipeline

Start Pipeline of end to AutoML, building of endpoint and show runDetail Widget in Jupyter notebook

![pipelinecreated](screenshots/pipelinecreated.png)

![pipelinecomplete_f](screenshots/pipelinecomplete_f.png)

![pipelineactive_f](screenshots/pipelineactive_f.png)

![jupyterrundetail_f](screenshots/jupyterrundetail_f.png)

## Screen Recording

https://www.youtube.com/watch?v=AFL9PlokgjA

## Future Suggestions
- Increase training of Automl to build additional models might drive better performance
- Collect more data to improve the model accuracy as it gives additional examples
- Data cleaning and feature engineering will be helpful in improving data quality and provide more information that the model may generalise better