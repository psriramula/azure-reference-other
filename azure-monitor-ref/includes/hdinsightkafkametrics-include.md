---
ms.service: azure-monitor
ms.topic: include
ms.date: 08/28/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: HDInsightKafkaMetrics
---


| Column | Type | Description |
|---|---|---|
| _BilledSize | real | The record size in bytes |
| ClusterName | string | Name of cluster. |
| CorrelationId | string | The ID for correlated events. Can be used to identify correlated events between multiple tables. |
| HostName | string | Name of host where log was emitted. |
| _IsBillable | string | Specifies whether ingesting the data is billable. When _IsBillable is `false` ingestion isn't billed to your Azure account |
| MetricDataType | string | CollectD datatype of the metric (e.g. gauge, counter, etc.). Determines how metric is portrayed over time. Please reference CollectD documentation for more information: https://collectd.org/wiki/index.php/Data_source . |
| MetricName | string | Name of the metric for the record (e.g. OfflinePartitionsCount, UnderReplicatedPartitions, LeaderCount, etc). |
| MetricNamespace | string | Category of metric (e.g. RequestMetrics, BrokerTopicMetrics, KafkaController, etc).  |
| MetricValue | real | Value of metric in the record. |
| OperationName | string | The operation associated with log record. |
| _ResourceId | string | A unique identifier for the resource that the record is associated with |
| SourceSystem | string | The type of agent the event was collected by. For example, `OpsManager` for Windows agent, either direct connect or Operations Manager, `Linux` for all Linux agents, or `Azure` for Azure Diagnostics |
| _SubscriptionId | string | A unique identifier for the subscription that the record is associated with |
| Tags | string | Information about the record. For example a record may be tagged with 'kafka.network' if it is a network related metric. |
| TenantId | string | The Log Analytics workspace ID |
| TimeGenerated | datetime | The timestamp (UTC) of when the log was generated. |
| Type | string | The name of the table |
