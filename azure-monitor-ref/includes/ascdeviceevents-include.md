---
ms.service: azure-monitor
ms.topic: include
ms.date: 08/28/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: ASCDeviceEvents
---


| Column | Type | Description |
|---|---|---|
| _BilledSize | real | The record size in bytes |
| CatalogId | string | The catalog ID of the device where the log event was generated. |
| CorrelationId | string | A unique correlation ID for the log event. |
| DeviceId | string | The ID of the device where the log event was generated. |
| DurationMs | int | The total duration (in milliseconds) for the log event. |
| _IsBillable | string | Specifies whether ingesting the data is billable. When _IsBillable is `false` ingestion isn't billed to your Azure account |
| Location | string | The location and region where the log event was generated. |
| OperationName | string | The Azure Sphere operation associated with the log event. |
| Properties | dynamic | Additional properties related to the log event. |
| _ResourceId | string | A unique identifier for the resource that the record is associated with |
| ResultDescription | string | The result description for the log event. |
| ResultType | string | The result type (success, failure) for the log event. |
| SourceSystem | string | The type of agent the event was collected by. For example, `OpsManager` for Windows agent, either direct connect or Operations Manager, `Linux` for all Linux agents, or `Azure` for Azure Diagnostics |
| _SubscriptionId | string | A unique identifier for the subscription that the record is associated with |
| TenantId | string | The Log Analytics workspace ID |
| TimeGenerated | datetime | Timestamp(UTC) when the log event was generated. |
| Type | string | The name of the table |
