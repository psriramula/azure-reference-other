---
ms.service: azure-monitor
ms.topic: include
ms.date: 08/28/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: AmlOnlineEndpointConsoleLog
---


| Column | Type | Description |
|---|---|---|
| _BilledSize | real | The record size in bytes |
| ContainerImageName | string | The name of the docker image running in the container where the log was generated. |
| ContainerName | string | The name of the container where the log was generated. |
| DeploymentName | string | The name of the deployment associated with the log record. |
| InstanceId | string | The ID of the instance that generated this log record. |
| _IsBillable | string | Specifies whether ingesting the data is billable. When _IsBillable is `false` ingestion isn't billed to your Azure account |
| Message | string | The content of the log. |
| OperationName | string | The operation associated with log record. |
| _ResourceId | string | A unique identifier for the resource that the record is associated with |
| SourceSystem | string | The type of agent the event was collected by. For example, `OpsManager` for Windows agent, either direct connect or Operations Manager, `Linux` for all Linux agents, or `Azure` for Azure Diagnostics |
| _SubscriptionId | string | A unique identifier for the subscription that the record is associated with |
| TenantId | string | The Log Analytics workspace ID |
| TimeGenerated | datetime | The timestamp (UTC) of when the log was generated. |
| Type | string | The name of the table |
