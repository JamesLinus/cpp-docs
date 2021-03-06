---
title: "no_namespace | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.reviewer: ""
ms.suite: ""
ms.technology:  
  - "cpp-tools"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "no_namespace"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "no_namespace attribute"
ms.assetid: 5d81b741-a558-451b-b493-1f3b18967337
caps.latest.revision: 4
author: "corob-msft"
ms.author: "corob"
manager: "ghogen"
translation.priority.ht: 
  - "cs-cz"
  - "de-de"
  - "es-es"
  - "fr-fr"
  - "it-it"
  - "ja-jp"
  - "ko-kr"
  - "pl-pl"
  - "pt-br"
  - "ru-ru"
  - "tr-tr"
  - "zh-cn"
  - "zh-tw"
---
# no_namespace
**C++ Specific**  
  
 Specifies that the namespace name is not generated by the compiler.  
  
## Syntax  
  
```  
no_namespace  
```  
  
## Remarks  
 The type-library contents in the `#import` header file are normally defined in a namespace. The namespace name is specified in the **library** statement of the original IDL file. If the `no_namespace` attribute is specified, then this namespace is not generated by the compiler.  
  
 If you want to use a different namespace name, then use the [rename_namespace](../preprocessor/rename-namespace.md) attribute instead.  
  
 **END C++ Specific**  
  
## See Also  
 [#import Attributes](../preprocessor/hash-import-attributes-cpp.md)   
 [#import Directive](../preprocessor/hash-import-directive-cpp.md)