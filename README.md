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

## What's the difference between workspace and an environment?

In order to create an environment you must have a workspace, in other words, you create your environment inside a workspace.
