---
title: "IDiaSymbol::get_sealed | Microsoft Docs"
ms.date: 11/15/2016
ms.prod: "visual-studio-dev14"
ms.technology: "vs-ide-debug"
ms.topic: reference
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "IDiaSymbol::get_sealed method"
ms.assetid: cd1fef1f-47de-47c7-885f-f6f0a9a07d8c
caps.latest.revision: 7
author: MikeJo5000
ms.author: mikejo
manager: jillfra
---
# IDiaSymbol::get_sealed
[!INCLUDE[vs2017banner](../../includes/vs2017banner.md)]

Retrieves a flag that specifies whether the class or method is sealed.  
  
## Syntax  
  
```cpp#  
HRESULT get_sealed(   
   BOOL* pRetVal)  
);  
```  
  
#### Parameters  
 `pRetVal`  
 [out] Returns `TRUE` if the class or method is sealed; otherwise, returns `FALSE`.  
  
## Return Value  
 If successful, returns `S_OK`; otherwise, returns `S_FALSE` or an error code.  
  
> [!NOTE]
>  A return value of `S_FALSE` means the property is not available for the symbol.  
  
## Remarks  
 A sealed class cannot be used as a base class. A sealed method cannot be overidden.  
  
## Requirements  
 Header: Dia2.h  
  
 Library: diaguids.lib  
  
 DLL: msdia100.dll  
  
## See Also  
 [IDiaSymbol](../../debugger/debug-interface-access/idiasymbol.md)
