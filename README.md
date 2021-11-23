# Azure Machine Learning Python SDK notebooks

Welcome to my Azure Machine Learning Python SDK notebooks repository!

## What is an Azure Machine Learning workspace?

Azure ML Workspace is the top-level resource for Azure Machine Learning. It is used to coordinate storage, databases, and compute resources providing added functionality for machine learning experimentation, deployment, inference, and the monitoring of deployed models.

![image](https://user-images.githubusercontent.com/25666677/143065957-41ae0c1f-abf9-46da-99d8-7a86702461cc.png)

### Create a workspace

1. Use the [Azure Machine Learning SDK for Python](https://docs.microsoft.com/en-us/azure/machine-learning/how-to-manage-workspace?tabs=python#create-a-workspace) to create a workspace on the fly from Python scripts or Jupyter notebooks

2. Use the [Azure portal](https://docs.microsoft.com/en-us/azure/machine-learning/how-to-manage-workspace?tabs=azure-portal#create-a-workspace) for a point-and-click interface to walk you through each step.


When you are running your code in Azure Notebooks or another Microsoft managed environment, the SDK is already installed.
Else: you should follow the steps in the [link](https://docs.microsoft.com/en-us/azure/machine-learning/how-to-configure-environment) to congfigure your environment.

## What are Azure Machine Learning environments?

Azure Machine Learning environments specify the Python packages, environment variables, and software settings around your training and scoring scripts. They are entities that exist in the workspace, they can be managed and versioned. 

Environments enable creating reproducible, auditable, and portable machine learning workflows across a variety of compute targets.

You can use an Environment object on your local compute to:

- Develop your training script.
- Reuse the same environment on Azure Machine Learning Compute for model training at scale.
- Deploy your model with that same environment.
- Revisit the environment in which an existing model was traine


To run an application, you need: code, runtime, system tools, system libraries and settings.  A container packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another.

Docker terms: 
- Images: Just a snapshot of your container.
- Dockerfile: That’s a yaml file that is used to build up your image. At the end you of this session you will have a yaml-file template and use it for with your own container specifications.
