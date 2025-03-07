---
ms.service: azure-monitor
ms.topic: include
ms.date: 11/09/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: Microsoft.Storage/storageAccounts/fileServices, naam
---
<!--
NOTE:  This content is automatically generated using API calls to Azure. 
Any edits made on these files will be overwritten in the next run of the script. 
There is no benefit in editing these files directly.  
-->
  
  
|Metric|Name in REST API|Unit|Aggregation|Dimensions|Time Grains|DS Export|
|---|---|---|---|---|---|---|
|**Availability**<p><p>The percentage of availability for the storage service or the specified API operation. Availability is calculated by taking the TotalBillableRequests value and dividing it by the number of applicable requests, including those that produced unexpected errors. All unexpected errors result in reduced availability for the storage service or the specified API operation. |`Availability` |Percent |Average, Minimum, Maximum |`GeoType`, `ApiName`, `Authentication`, `FileShare`|PT1M |Yes|
|**Egress**<p><p>The amount of egress data. This number includes egress to external client from Azure Storage as well as egress within Azure. As a result, this number does not reflect billable egress. |`Egress` |Bytes |Total, Average, Minimum, Maximum |`GeoType`, `ApiName`, `Authentication`, `FileShare`|PT1M |Yes|
|**File Capacity**<p><p>The amount of File storage used by the storage account. |`FileCapacity` |Bytes |Average |`FileShare`, `Tier`|PT1H |No|
|**File Count**<p><p>The number of files in the storage account. |`FileCount` |Count |Average |`FileShare`, `Tier`|PT1H |No|
|**File Share Capacity Quota**<p><p>The upper limit on the amount of storage that can be used by Azure Files Service in bytes. |`FileShareCapacityQuota` |Bytes |Average |`FileShare`|PT1H |No|
|**File Share Count**<p><p>The number of file shares in the storage account. |`FileShareCount` |Count |Average |\<none\>|PT1H |No|
|**Bandwidth by Max MiB/s**<p><p>The maximum number of used bandwidth in MiB/s at the lowest time granularity of 1-minute for the premium file share in the premium files storage account. |`FileShareMaxUsedBandwidthMiBps` |CountPerSecond |Maximum |`FileShare`|PT1M |No|
|**Transactions by Max IOPS**<p><p>The maximum number of used IOPS at the lowest time granularity of 1-minute for the premium file share in the premium files storage account. |`FileShareMaxUsedIOPS` |CountPerSecond |Maximum |`FileShare`|PT1M |No|
|**File Share Provisioned Bandwidth MiB/s**<p><p>The baseline number of provisioned bandwidth in MiB/s for the premium file share in the premium files storage account. This number is calculated based on the provisioned size (quota) of the share capacity. |`FileShareProvisionedBandwidthMiBps` |CountPerSecond |Average |`FileShare`|PT1H |No|
|**File Share Provisioned IOPS**<p><p>The baseline number of provisioned IOPS for the premium file share in the premium files storage account. This number is calculated based on the provisioned size (quota) of the share capacity. |`FileShareProvisionedIOPS` |CountPerSecond |Average |`FileShare`|PT1H |No|
|**File Share Snapshot Count**<p><p>The number of snapshots present on the share in storage account's Files Service. |`FileShareSnapshotCount` |Count |Average |`FileShare`|PT1H |No|
|**File Share Snapshot Size**<p><p>The amount of storage used by the snapshots in storage account's File service in bytes. |`FileShareSnapshotSize` |Bytes |Average |`FileShare`|PT1H |No|
|**Ingress**<p><p>The amount of ingress data, in bytes. This number includes ingress from an external client into Azure Storage as well as ingress within Azure. |`Ingress` |Bytes |Total, Average, Minimum, Maximum |`GeoType`, `ApiName`, `Authentication`, `FileShare`|PT1M |Yes|
|**Success E2E Latency**<p><p>The average end-to-end latency of successful requests made to a storage service or the specified API operation, in milliseconds. This value includes the required processing time within Azure Storage to read the request, send the response, and receive acknowledgment of the response. |`SuccessE2ELatency` |MilliSeconds |Average, Minimum, Maximum |`GeoType`, `ApiName`, `Authentication`, `FileShare`|PT1M |Yes|
|**Success Server Latency**<p><p>The average time used to process a successful request by Azure Storage. This value does not include the network latency specified in SuccessE2ELatency. |`SuccessServerLatency` |MilliSeconds |Average, Minimum, Maximum |`GeoType`, `ApiName`, `Authentication`, `FileShare`|PT1M |Yes|
|**Transactions**<p><p>The number of requests made to a storage service or the specified API operation. This number includes successful and failed requests, as well as requests which produced errors. Use ResponseType dimension for the number of different type of response. |`Transactions` |Count |Total |`ResponseType`, `GeoType`, `ApiName`, `Authentication`, `FileShare`, `TransactionType`|PT1M |Yes|