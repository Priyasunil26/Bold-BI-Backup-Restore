---
layout: post
title: Setup Database Manually or with Managed Service| Bold BI Docs
description: Discover how to set up a database either manually or with a managed service. Manual setup requires configuring and managing the database system, while a managed service handles tasks like provisioning, patching, backups, and scaling. Choose the method that suits your needs and resources best.
documentation: ug
---
# Deploy Database Server on AWS
Setting up a database can be done manually or by using a managed database service. Both approaches have their benefits and complexities, so it's essential to choose the one that best fits your needs and resources.

<ul>
<ol>

a. [Deploy Database Server Manually on AWS](self-deploy-database.md/#deploy-database-server-manually-on-aws)

b. [Deploy RDS instance on AWS ](self-deploy-database.md/#deploy-a-managed-database-server-on-aws)
</ol>
</ul>

## Deploy Database Server Manually on AWS
This guide provides detailed instructions on how to set up popular databases like PostgreSQL, MySQL, and SQL on both Windows and Linux VM.

**1. Setting up PostgreSQL in an EC2 Windows Instance**
- To set up a PostgreSQL database on a Windows VM, you can refer to the following [link](https://www.postgresqltutorial.com/postgresql-getting-started/install-postgresql/) for detailed installation steps.

- For installing a MySQL database in a Windows EC2 instance, refer to the steps outlined in this [guide](https://dev.mysql.com/doc/refman/8.3/en/windows-installation.html).

- To install an  SQL database in Windows EC2 instance, follow the instructions provided in this [guide](https://learn.microsoft.com/en-us/sql/database-engine/install-windows/install-sql-server?view=sql-server-ver16).

**2. Setting up PostgreSQL on Linux Instance**

- Before installing PostgreSQL on your Linux instance, ensure you review the [prerequisites](https://help.boldbi.com/deploying-bold-bi/deploying-in-linux/prerequisites-linux/). You can then use the package manager to [install PostgreSQL](https://www.postgresql.org/download/linux/ubuntu/).

- To install a MySQL database on a Linux EC2 instance, follow the steps provided in this [guide](https://www.devart.com/dbforge/mysql/how-to-install-mysql-on-linux/).

- To install an SQL database on Linux EC2 instance, follow the instructions provided in this [guide](https://phoenixnap.com/kb/sql-server-linux).

## Deploy a Managed Database Server on AWS
Setting up a managed database service on AWS involves configuring a database system.

- To create a PostgreSQL RDS in AWS, refer to this [link](https://aws.amazon.com/getting-started/hands-on/create-connect-postgresql-db/).

- To create a MySQL RDS in AWS, follow the instructions in this [link](https://aws.amazon.com/getting-started/hands-on/create-mysql-db/).

- To create a SQL RDS in AWS, follow the instructions in this [link](https://aws.amazon.com/getting-started/hands-on/create-microsoft-sql-db/).

