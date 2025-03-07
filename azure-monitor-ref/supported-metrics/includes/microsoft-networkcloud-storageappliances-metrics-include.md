---
ms.service: azure-monitor
ms.topic: include
ms.date: 11/09/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: Microsoft.NetworkCloud/storageAppliances, naam
---
<!--
NOTE:  This content is automatically generated using API calls to Azure. 
Any edits made on these files will be overwritten in the next run of the script. 
There is no benefit in editing these files directly.  
-->
  
  
|Metric|Name in REST API|Unit|Aggregation|Dimensions|Time Grains|DS Export|
|---|---|---|---|---|---|---|
|**Nexus Storage Alerts Total**<p><p>Number of alert events |`PurefaAlertsTotal` |Count |Average |`Severity`|PT1M |No|
|**Nexus Storage Array Avg Block Bytes**<p><p>Average block size |`PurefaArrayPerformanceAvgBlockBytes` |Bytes |Average |`Dimension`|PT1M |No|
|**Nexus Storage Array Bandwidth Bytes**<p><p>Array throughput in bytes per second |`PurefaArrayPerformanceBandwidthBytes` |Bytes |Average |`Dimension`|PT1M |No|
|**Nexus Storage Array IOPS**<p><p>Storage array IOPS |`PurefaArrayPerformanceIOPS` |Count |Average |`Dimension`|PT1M |No|
|**Nexus Storage Array Latency**<p><p>Storage array latency in microseconds |`PurefaArrayPerformanceLatencyUsec` |MilliSeconds |Average |`Dimension`|PT1M |No|
|**Nexus Storage Array Queue Depth**<p><p>Storage array queue depth |`PurefaArrayPerformanceQdepth` |Bytes |Average |\<none\>|PT1M |No|
|**Nexus Storage Array Capacity Bytes**<p><p>Storage array overall space capacity |`PurefaArraySpaceCapacityBytes` |Bytes |Average |\<none\>|PT1M |No|
|**Nexus Storage Array Space DDR**<p><p>Storage array overall data reduction |`PurefaArraySpaceDatareductionRatio` |Percent |Average |\<none\>|PT1M |No|
|**Nexus Storage Array Space Prov**<p><p>Storage array overall provisioned space |`PurefaArraySpaceProvisionedBytes` |Bytes |Average |\<none\>|PT1M |No|
|**Nexus Storage Array Space Used Bytes**<p><p>Storage Array overall used space |`PurefaArraySpaceUsedBytes` |Bytes |Average |`Dimension`|PT1M |No|
|**Nexus Storage HW Component Health**<p><p>Storage array hardware component health status |`PurefaHardwareComponentHealth` |Count |Average |`Component`, `Controller`, `Index`, `Chassis`|PT1M |No|
|**Nexus Storage Hardware Power Volts**<p><p>Storage array hardware power supply voltage |`PurefaHardwarePowerVolts` |Unspecified |Average |`Power Supply`|PT1M |No|
|**Nexus Storage Hardware Temp Celsius**<p><p>Storage array hardware temperature sensors |`PurefaHardwareTemperatureCelsius` |Unspecified |Average |`Controller`, `Sensor`|PT1M |No|
|**Nexus Storage Host Bandwidth Bytes**<p><p>Storage array host bandwidth in bytes per second |`PurefaHostPerformanceBandwidthBytes` |Bytes |Average |`Dimension`, `Host`|PT1M |No|
|**Nexus Storage Host IOPS**<p><p>Storage array host IOPS |`PurefaHostPerformanceIOPS` |Count |Average |`Dimension`, `Host`|PT1M |No|
|**Nexus Storage Host Latency**<p><p>Storage array host latency in microseconds |`PurefaHostPerformanceLatencyUsec` |MilliSeconds |Average |`Dimension`, `Host`|PT1M |No|
|**Nexus Storage Host Space Bytes**<p><p>Storage array host space in bytes |`PurefaHostSpaceBytes` |Bytes |Average |`Dimension`, `Host`|PT1M |No|
|**Nexus Storage Host Space DDR**<p><p>Storage array host volumes data reduction ratio |`PurefaHostSpaceDatareductionRatio` |Percent |Average |`Host`|PT1M |No|
|**Nexus Storage Host Space Size Bytes**<p><p>Storage array host volumes size |`PurefaHostSpaceSizeBytes` |Bytes |Average |`Host`|PT1M |No|
|**Nexus Storage Info (Preview)**<p><p>Storage array system information |`PurefaInfo` |Unspecified |Average |`Array Name`|PT1M |No|
|**Nexus Storage Volume Performance IOPS**<p><p>Storage array volume IOPS |`PurefaVolumePerformanceIOPS` |Count |Average |`Dimension`, `Volume`|PT1M |No|
|**Nexus Storage Vol Perf Latency**<p><p>Storage array volume latency in microseconds |`PurefaVolumePerformanceLatencyUsec` |MilliSeconds |Average |`Dimension`, `Volume`|PT1M |No|
|**Nexus Storage Vol Perf Throughput**<p><p>Storage array volume throughput |`PurefaVolumePerformanceThroughputBytes` |Bytes |Average |`Dimension`, `Volume`|PT1M |No|
|**Nexus Storage Volume Space Bytes**<p><p>Storage array volume space in bytes |`PurefaVolumeSpaceBytes` |Bytes |Average |`Dimension`, `Volume`|PT1M |No|
|**Nexus Storage Volume Space DDR**<p><p>Storage array overall data reduction |`PurefaVolumeSpaceDatareductionRatio` |Percent |Average |`Volume`|PT1M |No|
|**Nexus Storage Volume Space Size Bytes**<p><p>Storage array volumes size |`PurefaVolumeSpaceSizeBytes` |Bytes |Average |`Volume`|PT1M |No|