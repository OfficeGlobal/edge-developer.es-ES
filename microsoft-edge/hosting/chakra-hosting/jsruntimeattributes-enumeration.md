---
description: 'Atributos de un Runtime. '
title: JsRuntimeAttributes (enumeración) | Microsoft docs
ms.custom: ''
ms.date: 01/18/2017
ms.prod: microsoft-edge
ms.reviewer: ''
ms.suite: ''
ms.tgt_pltfrm: ''
ms.topic: reference
f1_keywords:
- jsrt/JsRuntimeAttributes
helpviewer_keywords:
- JsRuntimeAttributes enumeration
ms.assetid: f76d82e9-a695-4d6a-96c1-b3a4d27fed68
caps.latest.revision: 14
author: MSEdgeTeam
ms.author: msedgedevrel
manager: ''
ms.openlocfilehash: 9b8f6788f1de4988e3936701cfc742a564c92cfd
ms.sourcegitcommit: 6860234c25a8be863b7f29a54838e78e120dbb62
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/09/2020
ms.locfileid: "10574526"
---
# Enumeración JsRuntimeAttributes
Atributos de un Runtime.  
  
## Sintaxis  
  
```cpp  
enum JsRuntimeAttributes;  
```  
  
## Miembros  
  
### Los  
  
|Nombre|Descripción|  
|----------|-----------------|  
|`JsRuntimeAttributeAllowScriptInterrupt`|El motor en tiempo de ejecución debe admitir una interrupción de script confiable. Esto aumenta el número de lugares en los que el motor en tiempo de ejecución buscará una solicitud de interrupción de script a costa de una pequeña cantidad de rendimiento en tiempo de ejecución.|  
|`JsRuntimeAttributeDisableBackgroundWork`|El motor en tiempo de ejecución no realizará ningún trabajo (como la recolección de elementos no utilizados) en subprocesos en segundo plano.|  
|`JsRuntimeAttributeDisableEval`|El uso del `eval` `function` constructor or inicia una excepción.|  
|`JsRuntimeAttributeDisableNativeCodeGeneration`|El motor en tiempo de ejecución no generará código nativo.|  
|`JsRuntimeAttributeEnableExperimentalFeatures`|El motor en tiempo de ejecución habilitará todas las características experimentales.|  
|`JsRuntimeAttributeEnableIdleProcessing`|El anfitrión llama `JsIdle` , así que habilita el procesamiento de inactividad. De lo contrario, el motor en tiempo de ejecución administrará la memoria de forma ligeramente más agresiva.|  
|`JsRuntimeAttributeDispatchSetExceptionsToDebugger`|Las llamadas `JsSetException` también enviarán la excepción al depurador de script (si existe), lo que proporciona al depurador una oportunidad de interrumpir la excepción.|  
|`JsRuntimeAttributeNone`|Sin atributos especiales.|  
  
## Requisitos  
 **Encabezado:** jsrt. h  
  
## Consulta también  
 [Referencia (tiempo de ejecución de JavaScript)](../chakra-hosting/reference-javascript-runtime.md)