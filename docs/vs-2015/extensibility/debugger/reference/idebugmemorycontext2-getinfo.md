---
title: "IDebugMemoryContext2::GetInfo | Microsoft Docs"
ms.custom: ""
ms.date: 11/15/2016
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-sdk"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "IDebugMemoryContext2::GetInfo"
helpviewer_keywords: 
  - "GetInfo method"
  - "IDebugMemoryContext2::GetInfo method"
ms.assetid: 08c7f091-1816-4d64-8834-f9ecaac5c58d
caps.latest.revision: 14
ms.author: "gregvanl"
manager: "ghogen"
---
# IDebugMemoryContext2::GetInfo
[!INCLUDE[vs2017banner](../../../includes/vs2017banner.md)]

Retrieves a [CONTEXT_INFO](../../../extensibility/debugger/reference/context-info.md) structure that describes the context.  
  
## Syntax  
  
```cpp#  
HRESULT GetInfo(   
   CONTEXT_INFO_FIELDS dwFields,  
   CONTEXT_INFO*       pInfo  
);  
```  
  
```csharp  
int GetInfo(  
   enum_CONTEXT_INFO_FIELDS dwFields,   
   CONTEXT_INFO[]           pinfo  
);  
```  
  
#### Parameters  
 `dwFields`  
 [in] A combination of flags from the [CONTEXT_INFO_FIELDS](../../../extensibility/debugger/reference/context-info-fields.md) enumeration that indicate which fields of the [CONTEXT_INFO](../../../extensibility/debugger/reference/context-info.md) structure are to be fill in.  
  
 `pInfo`  
 [in, out] The `CONTEXT_INFO` structure that is filled in.  
  
## Return Value  
 If successful, returns `S_OK`; otherwise, returns an error code.  
  
## See Also  
 [IDebugMemoryContext2](../../../extensibility/debugger/reference/idebugmemorycontext2.md)   
 [CONTEXT_INFO_FIELDS](../../../extensibility/debugger/reference/context-info-fields.md)   
 [CONTEXT_INFO](../../../extensibility/debugger/reference/context-info.md)

