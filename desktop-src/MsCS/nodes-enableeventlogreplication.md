---
title: EnableEventLogReplication
description: Controls whether a node's system, application, and security event log entries are replicated in the event logs of all other cluster nodes.
audience: developer
author: REDMOND\\markl
manager: REDMOND\\markl
ms.assetid: c032f98e-bb27-445d-a7bf-c2ff1d484285
ms.prod: windows-server-dev
ms.technology: failover-clustering
ms.tgt_platform: multiple
keywords:
- EnableEventLogReplication Failover Cluster ,for nodes
- EnableEventLogReplication Failover Cluster
topic_type:
- apiref
api_name:
- EnableEventLogReplication
api_type:
- NA
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# EnableEventLogReplication

\[This property is available for use only in Windows Server 2003.\]

Controls whether a [node's](nodes.md) system, application, and security event log entries are replicated in the event logs of all other [*cluster*](https://www.bing.com/search?q=*cluster*) nodes.



| Attribute            | Value                                                                                                       |
|----------------------|-------------------------------------------------------------------------------------------------------------|
| Data type<br/> | **DWORD**<br/>                                                                                        |
| Access<br/>    | [Read/write](read-write-properties.md)<br/>                                                          |
| Structure<br/> | [**CLUSPROP\_DWORD**](/previous-versions/windows/desktop/api/ClusAPI/)<br/>                                                        |
| Minimum<br/>   | **FALSE** (0). The node's event log entries are not replicated to the other cluster nodes.<br/>       |
| Maximum<br/>   | **TRUE** (1). The node's event log entries are replicated event logs of all other cluster nodes.<br/> |
| Default<br/>   | **TRUE**<br/>                                                                                         |



 

## Remarks

The **EnableEventLogReplication** property only affects events logged to a node's system, application, and security logs.

## Examples

The property value portion of a [property list](property-lists.md) entry for **EnableEventLogReplication** can be set with the following example code:


```C++
CLUSPROP_DWORD PropertyValue;

PropertyValue.Syntax.dw = CLUSPROP_SYNTAX_LIST_VALUE_DWORD;
PropertyValue.cbLength  = sizeof(DWORD);
PropertyValue.dw        = FALSE;
```



## Requirements



|                                     |                                                                           |
|-------------------------------------|---------------------------------------------------------------------------|
| Minimum supported client<br/> | None supported<br/>                                                 |
| Minimum supported server<br/> | Windows Server 2003 Enterprise, Windows Server 2003 Datacenter<br/> |
| End of server support<br/>    | Windows Server 2003 Datacenter, Windows Server 2003 Enterprise<br/> |



## See also

<dl> <dt>

[**CLUSPROP\_DWORD**](/previous-versions/windows/desktop/api/ClusAPI/)
</dt> </dl>

 

 




