---
description: Una devolución de llamada llamada antes de la colección.
title: JsBeforeCollectCallback typedef | Microsoft docs
ms.custom: ''
ms.date: 01/18/2017
ms.prod: microsoft-edge
ms.reviewer: ''
ms.suite: ''
ms.tgt_pltfrm: ''
ms.topic: reference
ms.assetid: 58bece47-4e6d-49e7-a93d-b6a8f9928b41
caps.latest.revision: 6
author: MSEdgeTeam
ms.author: msedgedevrel
manager: ''
ms.openlocfilehash: 17f279c2d2ffcc8d02819994dddebfc22baa4cab
ms.sourcegitcommit: 6860234c25a8be863b7f29a54838e78e120dbb62
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/09/2020
ms.locfileid: "10573534"
---
# JsBeforeCollectCallback typedef
Una devolución de llamada llamada antes de la colección.  
  
## Sintaxis  
  
```cpp  
typedef void (CALLBACK *JsBeforeCollectCallback)(  
_In_opt_ void *callbackState  
);  
```  
  
#### Parámetros  
 callbackState  
 El estado pasado a JsSetBeforeCollectCallback.  
  
## Observaciones  
 Usa JsSetBeforeCollectCallback para registrar esta devolución de llamada.  
  
## Requisitos  
 **Encabezado:** jsrt. h  
  
## Consulta también  
 [Referencia (tiempo de ejecución de JavaScript)](../chakra-hosting/reference-javascript-runtime.md)