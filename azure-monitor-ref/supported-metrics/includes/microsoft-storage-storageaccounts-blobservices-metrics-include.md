---
ms.service: azure-monitor
ms.topic: include
ms.date: 10/18/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: Microsoft.Storage/storageAccounts/blobServices, naam
---
<!--
NOTE:  This content is automatically generated using API calls to Azure. 
Any edits made on these files will be overwritten in the next run of the script. 
There is no benefit in editing these files directly.  
-->
  
  
|Metric|Name in REST API|Unit|Aggregation|Dimensions|Time Grains|DS Export|
|---|---|---|---|---|---|---|
|**Availability**<p><p>The percentage of availability for the storage service or the specified API operation. Availability is calculated by taking the TotalBillableRequests value and dividing it by the number of applicable requests, including those that produced unexpected errors. All unexpected errors result in reduced availability for the storage service or the specified API operation. |`Availability` |Percent |Average, Minimum, Maximum |`GeoType`, `ApiName`, `Authentication`, `Tier`|PT1M |Yes|
|**Blob Capacity**<p><p>The amount of storage used by the storage account's Blob service in bytes. |`BlobCapacity` |Bytes |Average |`BlobType`, `Tier`|PT1H |No|
|**Blob Count**<p><p>The number of blob objects stored in the storage account. |`BlobCount` |Count |Average |`BlobType`, `Tier`|PT1H |No|
|**Blob Provisioned Size**<p><p>The amount of storage provisioned in the storage account's Blob service in bytes. |`BlobProvisionedSize` |Bytes |Average |`BlobType`, `Tier`|PT1H |No|
|**Blob Container Count**<p><p>The number of containers in the storage account. |`ContainerCount` |Count |Average |\<none\>|PT1H |Yes|
|**Egress**<p><p>The amount of egress data. This number includes egress to external client from Azure Storage as well as egress within Azure. As a result, this number does not reflect billable egress. |`Egress` |Bytes |Total, Average, Minimum, Maximum |`GeoType`, `ApiName`, `Authentication`, `Tier`|PT1M |Yes|
|**Index Capacity**<p><p>The amount of storage used by Azure Data Lake Storage Gen2 hierarchical index. |`IndexCapacity` |Bytes |Average |\<none\>|PT1H |No|
|**Ingress**<p><p>The amount of ingress data, in bytes. This number includes ingress from an external client into Azure Storage as well as ingress within Azure. |`Ingress` |Bytes |Total, Average, Minimum, Maximum |`GeoType`, `ApiName`, `Authentication`, `Tier`|PT1M |Yes|
|**Success E2E Latency**<p><p>The average end-to-end latency of successful requests made to a storage service or the specified API operation, in milliseconds. This value includes the required processing time within Azure Storage to read the request, send the response, and receive acknowledgment of the response. |`SuccessE2ELatency` |MilliSeconds |Average, Minimum, Maximum |`GeoType`, `ApiName`, `Authentication`, `Tier`|PT1M |Yes|
|**Success Server Latency**<p><p>The average time used to process a successful request by Azure Storage. This value does not include the network latency specified in SuccessE2ELatency. |`SuccessServerLatency` |MilliSeconds |Average, Minimum, Maximum |`GeoType`, `ApiName`, `Authentication`, `Tier`|PT1M |Yes|
|**Transactions**<p><p>The number of requests made to a storage service or the specified API operation. This number includes successful and failed requests, as well as requests which produced errors. Use ResponseType dimension for the number of different type of response. |`Transactions` |Count |Total |`ResponseType`, `GeoType`, `ApiName`, `Authentication`, `TransactionType`, `Tier`|PT1M |Yes|