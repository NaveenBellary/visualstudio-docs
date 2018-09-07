---
title: "IDebugDocumentPositionOffset2 | Microsoft Docs"
ms.custom: ""
ms.date: "2018-06-30"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-sdk"
ms.tgt_pltfrm: ""
ms.topic: "article"
helpviewer_keywords: 
  - "IDebugDocumentPositionOffset2 interface"
ms.assetid: f1b05db3-50d8-453f-a72f-e68b239236a4
caps.latest.revision: 8
ms.author: "gregvanl"
manager: "ghogen"
---
# IDebugDocumentPositionOffset2
[!INCLUDE[vs2017banner](../../../includes/vs2017banner.md)]

The latest version of this topic can be found at [IDebugDocumentPositionOffset2](https://docs.microsoft.com/visualstudio/extensibility/debugger/reference/idebugdocumentpositionoffset2).  
  
Represents a position in a source file as a character offset.  
  
## Syntax  
  
```  
IDebugDocumentPositionOffset2 : IUnknown  
```  
  
## Notes for Implementers  
 Implemented by the IDE and consumed by debug engines.  
  
## Methods  
 The following table shows the methods of `IDebugDocumentPositionOffset2`.  
  
|Method|Description|  
|------------|-----------------|  
|[GetRange](../../../extensibility/debugger/reference/idebugdocumentpositionoffset2-getrange.md)|Retrieves the range for the current document position.|  
  
## Remarks  
 This returns the same information as [GetRange](../../../extensibility/debugger/reference/idebugdocumentposition2-getrange.md) but in `char` offsets from the beginning of the document. This presents the document like it would exist on a disk, that is, a one-dimensional array of characters, instead of the line and column information that is ordinarily returned.  
  
## Requirements  
 Header: Msdbg.h  
  
 Namespace: Microsoft.VisualStudio.Debugger.Interop  
  
 Assembly: Microsoft.VisualStudio.Debugger.Interop.dll  
  
## See Also  
 [IDebugDocumentPosition2](../../../extensibility/debugger/reference/idebugdocumentposition2.md)
