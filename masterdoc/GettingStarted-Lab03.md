# Analytics in Microsoft Intelligent Data Platform (MIDP)

### Overall Estimated Duration : **90 Minutes**

## Overview

Azure Databricks and Power BI are key components in the Microsoft ecosystem for handling large datasets, enabling machine learning, and delivering business intelligence insights. This lab focuses on exploring these technologies by utilizing MLOps, sentiment analysis, and predictive analytics to drive business decisions at Wide World Importers. By leveraging Azure Databricks, you will deploy machine learning models for customer churn prediction and sentiment analysis, then operationalize them through Azure Machine Learning services. These models will be used to optimize marketing campaigns, sales forecasting, and improve customer engagement.

You will also utilize Power BI to derive actionable insights from enriched datasets stored in the Lakehouse. With the integration of campaign analytics, churn analysis, and website performance metrics, this lab will demonstrate how Wide World Importers can target the right customer segments, improve customer experiences, and forecast sales using data from the Lakehouse.

## Objective

**Exploring Machine Learning and Business Intelligence on the Lakehouse:** Learn to deploy machine learning models for customer churn prediction and sentiment analysis using Azure Databricks, and operationalize them through Azure Machine Learning services. Gain hands-on experience with integrating these models into business processes, such as campaign analytics and sales forecasting, to enhance decision-making. Additionally, explore how to leverage Power BI for analyzing data stored in the Lakehouse, uncovering insights into customer behavior, marketing effectiveness, and website performance. This process will develop skills in machine learning, data analytics, and the integration of business intelligence tools to drive data-driven outcomes.

## Prerequisites

Participants should have:

- **Basic Knowledge of Azure Databricks and Azure Machine Learning:** Familiarity with the Azure portal, creating and managing resources in Azure Databricks, and deploying machine learning models using Azure ML.
- **Understanding of Machine Learning Concepts:** Basic understanding of machine learning models, including training, validation, and deployment processes, specifically for tasks like churn prediction and sentiment analysis.
- **Basic Knowledge of Power BI:** Familiarity with Power BI for importing datasets, building reports, and analyzing data to derive business insights.
- **Familiarity with Data Storage Concepts:** Understanding of how data is organized and stored in a Lakehouse environment, especially within the context of Azure Databricks and Synapse Analytics.
- **Basic SQL Skills:** Ability to write and execute simple SQL queries for querying data in Azure Synapse Analytics and Databricks.

## Architecture

The lab architecture involves a structured flow where Azure Databricks is used to manage machine learning pipelines with MLflow, ensuring seamless data processing, model training, and deployment. A Databricks Delta Table acts as a centralized storage solution for structured data, enabling efficient access and analysis. MLflow is utilized to track experiments, register models, and manage their lifecycle. The trained models are operationalized as ML services in Azure Machine Learning, exposing REST endpoints for consumption. Business intelligence and advanced analytics tasks are performed using Power BI and SQL Analytics, providing actionable insights. This integrated flow supports efficient data processing, machine learning, and business intelligence workflows.

## Architecture Diagram

![Architecture Diagram](../media/image3100.png)

## Explanation of Components

The architecture for this lab involves the following key components:

- **Databricks Delta Table:** Acts as a centralized data storage layer, enabling high-performance data access and supporting machine learning tasks.

- **MLflow:** A framework for tracking machine learning experiments, registering models, and managing the model lifecycle. It supports different model flavors, such as Scikit-learn and XGBoost.

- **Model Registry:** A centralized repository within MLflow that allows versioning, approval, and lifecycle management of models.

- **Azure Machine Learning Services:** Provides a platform to deploy machine learning models as REST endpoints. It integrates with Azure Container Registry for hosting containerized models and ensures scalable and monitored deployment.

- **Power BI:** A business intelligence tool used to generate reports and dashboards, allowing users to derive actionable insights from the Lakehouse data.

- **SQL Analytics (Azure Synapse and Azure Databricks):** Tools for performing advanced SQL-based queries on data stored in the Lakehouse, facilitating deeper data exploration and insights.

## Getting Started with the Lab 

Once you're ready to dive in, your virtual machine and lab guide will be right at your fingertips within your web browser. 

> **Note:** We recommend having strong internet connectivity while performing the lab. Please ensure you are not connected to a VPN, which can slow down the lab-user experience.

![Architecture Diagram](../media/labstartpage2.png)

>**Note:** Please minimize the PowerShell window when it appears, do not close it, and wait 15 minutes for the process to complete. 

## Virtual Machine & Lab Guide

In the integrated environment, the lab VM serves as the designated workspace, while the lab guide is accessible on the right side of the screen.

**Note**: Kindly ensure that you are following the instructions carefully to ensure the lab runs smoothly and provides an optimal user experience.

## Exploring Your Lab Resources

To receive lab environment details, select the **Environment Details** tab. Additionally, the credentials will be sent to the email address you provided at registration.

   **Note:** If you see the pop-up **experience.cloudlabs.ai would like to access the Clipboard to copy text**, please click on **Allow**.

![Environment details](../media/labenvdet.png)
   
## Utilizing the Split Window Feature
 
For convenience, you can open the lab guide in a separate window by selecting the **Split Window** button from the Top right corner.
 
![splitwindow](../media/spl.png) 

## Lab Guide Zoom In/Zoom Out
 
To adjust the zoom level for the environment page, click the **A↕ : 100%** icon located next to the timer in the lab environment. 

![zoom](../media/zoom.png)  

## Managing Your Virtual Machine

Feel free to start, stop, or restart your virtual machine as needed from the **Resources** tab. Your experience is in your hands!

![resource](../media/res.png)  
  
## Let's Get Started with Azure Portal

1. On your virtual machine, click on the Azure Portal icon as shown below:

   ![Azurelogin](../media/labstartap.png)
   
1. You'll see the **Sign into Microsoft Azure** tab. Here, enter your credentials:
 
   - **Email/Username:** <inject key="AzureAdUserEmail"></inject>
 
       ![Enter Your Username](../media/click%20on%20next.png)
 
1. Next, provide your password:
 
   - **Password:** <inject key="AzureAdUserPassword"></inject>
 
       ![Enter Your Password](../media/06.png)

1. If you see the pop-up **Action Required**, keep default and then click on **Ask later**. If you see the pop-up **Help us protect your account**, click on **Skip for now(14 days until this is required)**, and then click on **Next**.

   >**Note:** You may see this pop-up multiple times, please proceed to **Skip**.

   ![Securitypopup](../media/ask-later-01.png)
 
1. If prompted to stay signed in, you can click "No."

1. If you see the pop-up **Sign in to sync data**, Click on **No,thanks.** 

1. If you see the pop-up **You have free Azure Advisor recommendations!**, close the window to continue the lab.

1. If a **Welcome to Microsoft Azure** popup window appears, click **Cancel** to skip the tour.

1. In the Azure portal, type **Resource groups (1)** in the search box and select **Resource groups (2)** from the results.

    ![In the search results pane, select the Resource group](../media/image1107.png)

13. On the **Resource groups** page, select **analyticsSolution**.

    ![In the filtered results, select the resource group](../media/image1109.png)

## Support Contact
 
The CloudLabs support team is available 24/7, 365 days a year, via email and live chat to ensure seamless assistance at any time. We offer dedicated support channels tailored specifically for both learners and instructors, ensuring that all your needs are promptly and efficiently addressed.

Learner Support Contacts:
- Email Support: cloudlabs-support@spektrasystems.com
- Live Chat Support: https://cloudlabs.ai/labs-support

Now, click on **Next** from the lower right corner to move on to the next page. 

![Securitypopup](../media/next.png)

### Happy Learning!!
