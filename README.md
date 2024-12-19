**Azure Data Factory Project**

**Overview**
This repository contains the infrastructure and configuration files for orchestrating and managing data workflows in Azure Data Factory (ADF). It includes the definitions for datasets, pipelines, linked services, dataflows, triggers, and configuration files for deployment. The project enables efficient ETL (Extract, Transform, Load) processes for integrating and processing data across various sources and destinations.

**Project Structure**
The project is organized into the following folders, each containing specific components of the Azure Data Factory configuration:

**dataflow/**
Contains dataflow definitions that define the transformations and processing logic applied to the data as it moves through the pipeline. Dataflows define the transformation steps such as filtering, aggregating, and mapping data between source and destination.

**dataset/**
Contains dataset definitions, which represent the structure of data in your data sources and sinks (e.g., Azure SQL tables, files in Blob Storage, or data in Data Lake). Datasets are used by pipelines to interact with the actual data.

**factory/**
Contains configurations related to the Azure Data Factory instance, including references to other resources, linked services, and global parameters. This is where you configure the overall ADF instance and manage factory-level settings.

**linkedService/**
Contains linked service configurations, which define the connections to external data sources or destinations such as databases, storage accounts, and other services. Linked services allow ADF to interact with different data stores and services.

**pipeline/**
Contains pipeline definitions that define the workflows for data movement and transformation. Pipelines consist of activities that interact with datasets and linked services to orchestrate data processing steps.

**trigger/**
Contains trigger configurations that automate the execution of pipelines based on schedules, events, or other triggers. Triggers help to automate ETL workflows without manual intervention.

**publish_config.json**
Contains the configuration settings for publishing and deploying resources to the Azure Data Factory instance. This file is used during deployment to ensure the correct version of all components is published to the target environment.
