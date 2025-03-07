---
ms.service: azure-monitor
ms.topic: include
ms.date: 10/18/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: Microsoft.ConnectedCache/CacheNodes, naam
---
<!--
NOTE:  This content is automatically generated using API calls to Azure. 
Any edits made on these files will be overwritten in the next run of the script. 
There is no benefit in editing these files directly.  
-->
  
  
|Metric|Name in REST API|Unit|Aggregation|Dimensions|Time Grains|DS Export|
|---|---|---|---|---|---|---|
|**Egress Mbps**<p><p>Egress Throughput |`egressbps` |BitsPerSecond |Average |`cachenodeid`|PT1M |Yes|
|**Cache Efficiency**<p><p>Cache Efficiency |`hitRatio` |Percent |Average |`cachenodeid`|PT1M |Yes|
|**Hits**<p><p>Count of hits |`hits` |Count |Count |`cachenodeid`|PT1M |Yes|
|**Hit Mbps**<p><p>Hit Throughput |`hitsbps` |BitsPerSecond |Average |`cachenodeid`|PT1M |Yes|
|**Misses**<p><p>Count of misses |`misses` |Count |Count |`cachenodeid`|PT1M |Yes|
|**Miss Mbps**<p><p>Miss Throughput |`missesbps` |BitsPerSecond |Average |`cachenodeid`|PT1M |Yes|