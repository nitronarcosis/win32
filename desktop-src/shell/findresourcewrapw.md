---
Description: Determines the location of a resource with the specified type and name, in the specified module.
ms.assetid: d8322430-5064-407e-8b89-b86b75bf139e
title: FindResourceWrapW function
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# FindResourceWrapW function

\[**FindResourceWrapW** is available for use in Windows XP. It may not be available in subsequent versions. You should use [**FindResourceW**](https://msdn.microsoft.com/windows/desktop/00f14551-5381-4499-a13a-86f15dd4e618) instead.\]

Determines the location of a resource with the specified type and name, in the specified module.

> [!Note]  
> **FindResourceWrapW** is a wrapper for the **FindResourceW** function. See [**FindResource**](https://msdn.microsoft.com/windows/desktop/00f14551-5381-4499-a13a-86f15dd4e618) for further usage notes.

 

## Syntax


```C++
HRSRC FindResourceWrapW(
  _In_ HMODULE hModule,
  _In_ LPCWSTR lpName,
  _In_ LPCWSTR lpType
);
```



## Parameters

<dl> <dt>

*hModule* \[in\]
</dt> <dd>

Type: **HMODULE**

A handle to the module whose executable file contains the resource. A value of **NULL** specifies the module handle associated with the image file that the operating system used to create the current process.

</dd> <dt>

*lpName* \[in\]
</dt> <dd>

Type: **LPCWSTR**

The name of the resource. For more information, see [**FindResource**](https://msdn.microsoft.com/windows/desktop/00f14551-5381-4499-a13a-86f15dd4e618).

</dd> <dt>

*lpType* \[in\]
</dt> <dd>

Type: **LPCWSTR**

A pointer to a string that specifies the resource type. For more information, see [**FindResource**](https://msdn.microsoft.com/windows/desktop/00f14551-5381-4499-a13a-86f15dd4e618).

</dd> </dl>

## Return value

Type: **HRSRC**

If the function succeeds, the return value is a handle to the specified resource's information block. To obtain a handle to the resource, pass this handle to the [**LoadResource**](https://msdn.microsoft.com/windows/desktop/4c91f571-505d-4959-b337-8f26c91fc573) function.

If the function fails, the return value is **NULL**. To get extended error information, call the [**GetLastError**](https://msdn.microsoft.com/windows/desktop/d852e148-985c-416f-a5a7-27b6914b45d4) function.

## Remarks

If you need to specify a particular localization, use the [**FindResourceEx**](https://msdn.microsoft.com/windows/desktop/3a9bfcca-68d8-4705-914b-dae844b5e0c3) function rather than **FindResourceWrapW**.

**FindResourceWrapW** provides the ability to use Unicode strings in older operating systems. The preferred method is to use [**FindResourceW**](https://msdn.microsoft.com/windows/desktop/00f14551-5381-4499-a13a-86f15dd4e618) in conjunction with the Microsoft Layer for Unicode (MSLU).

**FindResourceWrapW** must be called directly from Shlwapi.dll, using ordinal 66.

## Requirements



|                                     |                                                                                                               |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 2000 Professional, Windows XP \[desktop apps only\]<br/>                                        |
| Minimum supported server<br/> | Windows Server 2003 \[desktop apps only\]<br/>                                                          |
| Header<br/>                   | <dl> <dt>None</dt> </dl>                               |
| DLL<br/>                      | <dl> <dt>Shlwapi.dll (version 5.0 or later)</dt> </dl> |
| Unicode and ANSI names<br/>   | **FindResourceWrapW** (Unicode)<br/>                                                                    |



## See also

<dl> <dt>

[**FindResource**](https://msdn.microsoft.com/windows/desktop/00f14551-5381-4499-a13a-86f15dd4e618)
</dt> </dl>

 

 



