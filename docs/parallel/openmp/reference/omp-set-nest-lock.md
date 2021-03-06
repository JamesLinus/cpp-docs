---
title: "omp_set_nest_lock | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.reviewer: ""
ms.suite: ""
ms.technology:  
  - "cpp-windows"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "omp_set_nest_lock"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "omp_set_nest_lock OpenMP function"
ms.assetid: b98ed889-ff8e-4217-a3e9-3993ed8699af
caps.latest.revision: 9
author: "mikeblome"
ms.author: "mblome"
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
# omp_set_nest_lock
Blocks thread execution until a lock is available.  
  
## Syntax  
  
```  
void omp_set_nest_lock(  
   omp_nest_lock_t *lock  
);  
```  
  
## Remarks  
 where,  
  
 `lock`  
 A variable of type [omp_nest_lock_t](../../../parallel/openmp/reference/omp-nest-lock-t.md) that was initialized with [omp_init_nest_lock](../../../parallel/openmp/reference/omp-init-nest-lock.md).  
  
## Remarks  
 For more information, see [3.2.3 omp_set_lock and omp_set_nest_lock Functions](../../../parallel/openmp/3-2-3-omp-set-lock-and-omp-set-nest-lock-functions.md).  
  
## Examples  
 See [omp_init_nest_lock](../../../parallel/openmp/reference/omp-init-nest-lock.md) for an example of using `omp_set_nest_lock`.  
  
## See Also  
 [Functions](../../../parallel/openmp/reference/openmp-functions.md)