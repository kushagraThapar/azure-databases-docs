---
title: How to create databases
description: This article describes how to create and manage databases on Azure Database for MySQL - Flexible Server.
author: SudheeshGH
ms.author: sunaray
ms.reviewer: maghan
ms.date: 06/18/2024
ms.service: azure-database-mysql
ms.subservice: flexible-server
ms.topic: how-to
---

# Create and manage databases for Azure Database for MySQL - Flexible Server

[!INCLUDE[applies-to-mysql-flexible-server](../includes/applies-to-mysql-flexible-server.md)]

This article contains information about creating, listing, and deleting MySQL databases on Azure Database for MySQL Flexible Server. 

## Prerequisites
Before completing the tasks, you must have
- Created an Azure Database for MySQL Flexible Server instance using [Azure portal](./quickstart-create-server-portal.md) <br/> or [Azure CLI](./quickstart-create-server-cli.md).
- Sign in to [Azure portal](https://portal.azure.com).


## List your databases
To list all your databases on Azure Database for MySQL Flexible Server:
- Open the **Overview** page of your Azure Database for MySQL Flexible Server instance.
- Select **Databases** from the settings on left navigation menu. 

> :::image type="content" source="media/how-to-create-manage-databases/databases-view-mysql-flexible-server.png" alt-text="Screenshot showing how to list all the databases on Azure Database for MySQL Flexible Server.":::

## Create a database
To create a database on Azure Database for MySQL Flexible Server:

- Select **Databases** from the settings on left navigation menu. 
- Click on **Add** to create a database. Provide the database name, charset and collation settings for this database.
- Click on  **Save** to complete the task. 

> :::image type="content" source="media/how-to-create-manage-databases/create-database-azure-mysql-flexible-server.png" alt-text="Screenshot showing how to create a database on Azure Database for MySQL Flexible Server."::: 

## Delete a database
To delete a database on Azure Database for MySQL Flexible Server:

- Select **Databases** from the settings on left navigation menu. 
- Click on **testdatabase1** to select the database. You can select multiple databases to delete at the same time. 
- Click on  **Delete** to complete the task. 

> :::image type="content" source="media/how-to-create-manage-databases/delete-database-on-mysql-flexible-server.png" alt-text="Screenshot showing how to delete a database on Azure Database for MySQL Flexible Server."::: 

## Next steps

Learn how to [manage users](../howto-create-users.md)
