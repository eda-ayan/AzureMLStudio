# Azure Machine Learning Python SDK notebooks

Welcome to my Azure Machine Learning Python SDK notebooks repository!

## What is an Azure Machine Learning workspace?

Azure ML Workspace is the top-level resource for Azure Machine Learning. It is used to coordinate storage, databases, and compute resources providing added functionality for machine learning experimentation, deployment, inference, and the monitoring of deployed models.

![image](https://user-images.githubusercontent.com/25666677/143065957-41ae0c1f-abf9-46da-99d8-7a86702461cc.png)

### Creating a workspace using Azure Portal

1. Sign in to the Azure portal by using the credentials for your Azure subscription.

2. In the upper-left corner of Azure portal, select + Create a resource.
![image](https://user-images.githubusercontent.com/25666677/143066661-2454caf7-e520-458d-9ef5-c076f84e7c20.png)

3. Use the search bar to find Machine Learning.

4. Select Machine Learning.

5. In the Machine Learning pane, select Create to begin.

6. Provide the following information to configure your new workspace:

  <img src="https://user-images.githubusercontent.com/25666677/143066944-3c8e0fdc-1882-492b-9863-bf1960bfe586.png" width=70% height=70% /> 



When you are running your code in Azure Notebooks or another Microsoft managed environment, the SDK is already installed.
Else: you should follow the steps in the [link](https://docs.microsoft.com/en-us/azure/machine-learning/how-to-configure-environment) to congfigure your environment.

## What's the difference between workspace and an environment?

In order to create an environment you must have a workspace, in other words, you create your environment inside a workspace.
