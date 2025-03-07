---
title: Azure Monitor Logs reference - AzureActivityV2
description: Reference for AzureActivityV2 table in Azure Monitor Logs.
ms.topic: reference
ms.service: azure-monitor
ms.subservice: logs
ms.author: bwren
author: bwren
ms.date: 3/29/2021
---

# AzureActivityV2

 Azure activity logs.

## Categories

- Audit
## Solutions

- LogManagement
## Resource types

- Azure activity Log V2




## Columns

|Column|Type|Description|
|---|---|---|
|ActivityStatusValue|string|Status of the operation in display-friendly format. Common values include Started, In Progress, Succeeded, Failed, Active, Resolved.|
|ActivitySubstatusValue|string|Substatus of the operation in display-friendly format. E.g. OK (HTTP Status Code: 200).|
|Authorization|string|Blob of RBAC properties of the event. Usually includes the action, role, and scope properties.|
|AzureResourceGroup|string|Resource group name of the impacted resource.|
|AzureResourceId|string|Resource ID of the impacted resource.|
|AzureSubscriptionId|string|Subscription ID of the impacted resource.|
|AzureTenantId|string|The Azure tenant ID of the impacted resource.|
|Caller|string|Unique identifier of the caller.|
|CallerIpAddress|string|IP address of the user who has performed the operation UPN claim or SPN claim based on availability.|
|CategoryValue|string|Category of the activity log e.g. Administrative, Policy, Security.|
|Claims|string|The JWT token used by Active Directory to authenticate the user or application to perform this operation in Resource Manager.|
|CorrelationId|string|Usually a GUID in the string format. Events that share a correlationId belong to the same uber action.|
|Description|string|The description of the operation|
|EventDataId|string|Unique identifier of an event.|
|EventSubmissionTimestamp|datetime|Timestamp when the event became available for querying.|
|Hierarchy|string|Management group hierarchy of the management group or subscription that event belongs to.|
|HTTPRequest|string|Blob describing the Http Request. Usually includes the clientRequestId, clientIpAddress, and method (HTTP method. For example, PUT).|
|Level|string|Level of the event. One of the following values: Critical, Error, Warning, Informational and Verbose.|
|Misc|dynamic|Miscellaneous column for internal use.|
|MoboTenantId|string|ID of the activity logs workspace that stores this record.|
|OperationId|string|Unique identifier of the operation.|
|OperationNameValue|string|Identifier of the operation e.g. Microsoft.Storage/storageAccounts/listAccountSas/action.|
|PropertiedBackCompat|string|Set of `<Key Value>` pairs (i.e. Dictionary) describing the details of the event. Used for back compat with legacy activity logs|
|Properties|string|Set of `<Key Value>` pairs (i.e. Dictionary) describing the details of the event.|
|_ResourceId|string|A unique identifier for the resource that the record is associated with|
|ResourceProviderValue|string|Id of the resource provider for the impacted resource - e.g. Microsoft.Storage.|
|SourceSystem|string|Azure is used always for AzureActivity.|
|_SubscriptionId|string|A unique identifier for the subscription that the record is associated with|
|TenantId|string||
|TimeGenerated|datetime|Timestamp when the event was generated by the Azure service processing the request.|
|Type|string|The name of the table|
