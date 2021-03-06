---
title: "IDiaPropertyStorage::ReadDWORD | Microsoft Docs"
ms.custom: ""
ms.date: 11/15/2016
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-debug"
ms.tgt_pltfrm: ""
ms.topic: "article"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "IDiaPropertyStorage::ReadDWORD"
ms.assetid: 5f4c034e-a9d3-4560-94b5-ede524741439
caps.latest.revision: 11
author: "mikejo5000"
ms.author: "mikejo"
manager: "ghogen"
---
# IDiaPropertyStorage::ReadDWORD
[!INCLUDE[vs2017banner](../../includes/vs2017banner.md)]

Reads `DWORD` values in a property set.  
  
## Syntax  
  
```cpp#  
HRESULT ReadDWORD (   
   PROPID id,  
   DWORD* pValue  
);  
```  
  
#### Parameters  
 `id`  
 [in] Identifier of the property to be read (`PROPID` is defined in WTypes.h as a `ULONG`).  
  
 `pValue`  
 [out] Returns the property value.  
  
## Return Value  
 If successful, returns `S_OK`; otherwise returns an error code. Returns `E_INVALIDARG` if the property is not of type `DWORD`.  
  
## Remarks  
 A `DWORD` is defined by Windows as a 32-bit unsigned integer.  
  
## See Also  
 [IDiaPropertyStorage](../../debugger/debug-interface-access/idiapropertystorage.md)



