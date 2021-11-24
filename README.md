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

Azure Machine Learning builds environment definitions into Docker images and conda environments. 

You can create an environment [using Azure Machine Learning studio](https://docs.microsoft.com/en-us/azure/machine-learning/how-to-manage-environments-in-studio) or [using Python scripts](https://docs.microsoft.com/en-us/azure/machine-learning/how-to-use-environments)

## Create an environment using Azure Machine Learning Studio

To create an environment:

1. Open your workspace in Azure Machine Learning studio.
2. On the left side, select Environments.
3. Select the Custom environments tab.
4. Select the Create button.

![image](https://user-images.githubusercontent.com/25666677/143198540-816b57be-3043-4665-b21f-c28bae568c12.png)

You can use both Conda and Docker layers while creating an environment.

Once the environment is created, you can view and edit the environment details by clicking on the name.

![image](https://user-images.githubusercontent.com/25666677/143198694-9de940af-2380-49fc-bc9b-2eb3c4579777.png)

Use the dropdown menu to select different versions of the environment. Here you can view metadata and the contents of the environment through its Docker and Conda layers.
Keep in mind that any changes to the Docker or Conda sections will create a new version of the environment.

## Create an environment using Python script

### Instantiate an environment object

```python

from azureml.core.environment import Environment
Environment(name="myenv")

```

Docker terms: 
- Images: Just a snapshot of your container.
- Dockerfile: That’s a yaml file that is used to build up your image. At the end you of this session you will have a yaml-file template and use it for with your own container specifications.



More information on [creating environments](https://docs.microsoft.com/en-us/azure/machine-learning/how-to-use-environments)
