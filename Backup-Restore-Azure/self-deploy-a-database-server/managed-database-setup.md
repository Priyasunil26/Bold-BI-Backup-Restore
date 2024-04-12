---
layout: post
title: Configure a Managed Database Service| Bold BI Documentation
description: Discover how to set up a managed database service on Microsoft Azure involves configuring a database system provided by Azure. These services manage tasks such as backups and scaling, allowing users to focus on their applications without worrying about the infrastructure.
platform: bold-bi
documentation: ug
---
# Configure a Managed Database Service
Setting up a managed database service on Microsoft Azure, which involves configuring a database system provided by Azure. 

#### Setting up an Azure Database for PostgreSQL

  To set up a PostgreSQL database on Azure with the desired configurations, follow these detailed steps:

  - Click on `create a resource`, navigate to the services list, select `Database`, and then choose the Azure Database for PostgreSQL option.
    ![Create Resource](../images/create-resource.png)
    ![Azure Database](../images/search-database.png)
  - Proceed to enter the required information to establish your Database:
    - In the basic settings, select your subscription, pick an existing resource group or make a new one, input a name for your PostgreSQL server, and select a region.
      ![Datase Basic Setting](../images/Basic-setting-database.png)
      ![alt text](../images/Basic-setting-database.png)
    - For server settings, select a pricing tier (such as Basic, General Purpose, or Memory Optimized), choose a PostgreSQL version, and create a username and password for the server admin. In the compute + storage section, activate the option for Geo-redundancy.
      ![Admin Setting](../images/admin-setting-database.png)
      ![Compute and storage](../images/Compute-storage.png)
    - In the networking section, select your preferred connectivity method (like public or private endpoint), set up firewall rules, and ensure the box is checked to permit server access. Afterward, click the `Review and create` button.
      ![Network Setting](../images/network-setting-database.png)
    - Use the server name, username, and password you chose during setup to connect to your new database.
      ![Database overview](../images/overview-database.png)
  - For further guidance, you can refer to the following link: [Quickstart: Create an Azure Database for PostgreSQL server in the Azure portal](https://learn.microsoft.com/en-us/azure/postgresql/flexible-server/quickstart-create-server-portal)

**Instructions:** 
  - To create a MySQL database in Azure, follow the instructions in this [link](https://learn.microsoft.com/en-us/azure/mysql/flexible-server/quickstart-create-server-portal).
  - To create a MS SQL database in Azure, follow the instructions in this [link](https://learn.microsoft.com/en-us/azure/azure-sql/database/single-database-create-quickstart?view=azuresql&tabs=azure-portal).