---
Description: Notifies the callback object that an event has taken place that affects one of its items. Used by IShellFolderViewCB::MessageSFVCB.
title: SFVM_FSNOTIFY message
ms.topic: reference
ms.date: 05/31/2018
ms.assetid: ff159c35-afdf-4147-8dd6-7febd9519b18
api_name: 
 - SFVM_FSNOTIFY
api_type: 
 - HeaderDef
api_location: 
 - Shlobj.h
topic_type: 
 - APIRef
 - kbSyntax

---

# SFVM\_FSNOTIFY message

Notifies the callback object that an event has taken place that affects one of its items. Used by [**IShellFolderViewCB::MessageSFVCB**](https://msdn.microsoft.com/en-us/library/Bb774968(v=VS.85).aspx).


```C++
SFVM_FSNOTIFY 

    wParam = (WPARAM)(LPCITEMIDLIST) pidl;

    lParam = (LPARAM)(DWORD) lEvent;

            
```



## Parameters

<dl> <dt>

*pidl* \[in\]
</dt> <dd>

The PIDL of the affected item.

</dd> <dt>

*lEvent* \[in\]
</dt> <dd>

A SHCNE value that indicates which event occurred. For a list of possible values, see [**SHChangeNotify**](/windows/desktop/api/shlobj_core/nf-shlobj_core-shchangenotify).

</dd> </dl>

## Requirements



|                                     |                                                                                     |
|-------------------------------------|-------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 2000 Professional \[desktop apps only\]<br/>                          |
| Minimum supported server<br/> | Windows 2000 Server \[desktop apps only\]<br/>                                |
| Header<br/>                   | <dl> <dt>Shlobj.h</dt> </dl> |



 

 




