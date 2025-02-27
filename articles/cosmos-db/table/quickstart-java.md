---
title: Quickstart - Java client library
titleSuffix: Azure Cosmos DB for Table
description: Deploy a Java web application that uses the Azure SDK for Java to interact with Azure Cosmos DB for Table data in this quickstart.
author: seesharprun
ms.author: sidandrews
ms.reviewer: sasinnat
ms.service: azure-cosmos-db
ms.subservice: table
ms.devlang: java
ms.topic: quickstart-sdk
ms.date: 10/24/2024
ms.custom: devx-track-java, devx-track-extended-azdevcli
# CustomerIntent: As a developer, I want to learn the basics of the Java library so that I can build applications with Azure Cosmos DB for Table.
---

# Quickstart: Azure Cosmos DB for Table library for Java

[!INCLUDE[Table](../includes/appliesto-table.md)]

[!INCLUDE[Developer Quickstart selector](includes/quickstart/dev-selector.md)]

This quickstart shows how to get started with the Azure Cosmos DB for Table from a Java application. The Azure Cosmos DB for Table is a schemaless data store allowing applications to store structured table data in the cloud. You learn how to create tables, rows, and perform basic tasks within your Azure Cosmos DB resource using the Azure SDK for Java.

[API reference documentation](/java/api/com.azure.data.tables) | [Library source code](https://github.com/Azure/azure-sdk-for-java/tree/main/sdk/tables/azure-data-tables) | [Package (Maven)](https://mvnrepository.com/artifact/com.azure/azure-data-tables) | [Azure Developer CLI](/azure/developer/azure-developer-cli/overview)

## Prerequisites

- An Azure account with an active subscription. [Create an account for free](https://azure.microsoft.com/free/?WT.mc_id=A261C142F).
- [Azure Developer CLI](/azure/developer/azure-developer-cli/install-azd)
- [Docker Desktop](https://www.docker.com/products/docker-desktop/)

## Initialize the project

Use the Azure Developer CLI (`azd`) to create an Azure Cosmos DB for Table account and deploy a containerized sample application. The sample application uses the client library to manage, create, read, and query sample data.

1. Open a terminal in an empty directory.

1. If you're not already authenticated, authenticate to the Azure Developer CLI using `azd auth login`. Follow the steps specified by the tool to authenticate to the CLI using your preferred Azure credentials.

    ```azurecli
    azd auth login
    ```

1. Use `azd init` to initialize the project.

    ```azurecli
    azd init --template cosmos-db-table-java-quickstart
    ```

1. During initialization, configure a unique environment name.

1. Deploy the Azure Cosmos DB account using `azd up`. The Bicep templates also deploy a sample web application.

    ```azurecli
    azd up
    ```

1. During the provisioning process, select your subscription, desired location, and target resource group. Wait for the provisioning process to complete. The process can take **approximately five minutes**.

1. Once the provisioning of your Azure resources is done, a URL to the running web application is included in the output.

    ```output
    Deploying services (azd deploy)
    
      (✓) Done: Deploying service web
    - Endpoint: <https://[container-app-sub-domain].azurecontainerapps.io>
    
    SUCCESS: Your application was provisioned and deployed to Azure in 5 minutes 0 seconds.
    ```

1. Use the URL in the console to navigate to your web application in the browser. Observe the output of the running app.

    :::image type="content" source="media/quickstart/dev-web-application.png" alt-text="Screenshot of the running web application.":::

## Clean up resources

When you no longer need the sample application or resources, remove the corresponding deployment and all resources.

```azurecli
azd down
```

## Related content

- [.NET Quickstart](quickstart-dotnet.md)
- [Node.js Quickstart](quickstart-nodejs.md)
- [Python Quickstart](quickstart-python.md)
