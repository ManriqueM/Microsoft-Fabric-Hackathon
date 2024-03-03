# Microsoft-Fabric-Hackathon
<!-- ABOUT THE PROJECT -->
## Leveraging distinct Microsoft Fabric (and Copilot capabilities) for Anomaly Detection, using a synthetic dataset created with Azure OpenAI

Project submitted for the "Hack Together: The Microsoft Fabric Global AI Hack" (https://github.com/microsoft/Hack-Together-Fabric-AI)

For more details about this submission, please refer to: (https://example.com)

### Background

*"Microsoft Fabric is an all-in-one analytics solution for enterprises that covers everything from data movement to data science, Real-Time Analytics, and business intelligence. It offers a comprehensive suite of services, including data lake, data engineering, and data integration, all in one place. With Fabric, you don't need to piece together different services from multiple vendors. Instead, you can enjoy a highly integrated, end-to-end, and easy-to-use product that is designed to simplify your analytics needs. The platform is built on a foundation of Software as a Service (SaaS), which takes simplicity and integration to a whole new level".* [^1]

[^1]: Source: https://learn.microsoft.com/en-us/fabric/get-started/microsoft-fabric-overview

### Project Description

This project leverages multiple Microsoft Fabric components to approach the problem of anomaly detection. It approaches the problem from 4 different angles: 
- within PowerBI
- with KQL visuals
- running a specific model within Notebook
- creating a "low-code" model with the help of Azure OpenAI

Also, the data for this project was generated using Azure Open AI and to make it more realistic, it's based on a Global Retail Electronics Store. 

### Project Components

The description below shows the components used in the project.
`Workspace` `Lakehouse` `Notebooks` `AzureOpenAI` 
`SQL Analytics Endpoint` `Semantic Model` `PowerBI (and PBI Desktop)` `Copilot for PowerBI`
`KQL Database (using shortcuts)` `KQL Dataset`

The image below, from the Lineage view, summarizes how these components are being used together (the blue boxes were used to create the data and the red boxes are the different outputs).

![Test](images/Description.png)

This is how Azure OpenAI and Copilot were leveraged:
- **Azure OpenAI**:
	- Creating a base dataset (3 dimension tables and 1 fact table) based on dataspecs
	- Enhancing the base dataset and adapting it for a Global Retail Electronics Store
	- Creating a "low-code" anomaly detection model
- **Copilot**:
	- Auto-create Report Feature in PowerBI, to create a base report.
	- Using PowerBI Desktop, to adjust the .pbix and include AI features (Smart Narratives, also to use Anomaly Detection and Explain By feature)

### Development Process
All scripts are included in the Scripts subfolder from this repository.

### 01 - Create Base Dataset leveraging AzureOpenAI and Data_Specs
Please refer to this link: Scripts/Create_Dataset_Azure_OpenAI.ipynb

### 02 - Enhance Base Dataset, adapt to historical sales for a Global Retail Electronics Store and load delta tables to Lakehouse
Please refer to this link: Scripts/Create_Dataset_Azure_OpenAI.ipynb

### Outputs


<p align="right">(<a href="#readme-top">back to top</a>)</p>