---
description: Hospedar contenido web en la aplicación Win32 con el control Microsoft Edge WebView2
title: Microsoft Edge WebView2 para aplicaciones Win32
author: MSEdgeTeam
ms.author: msedgedevrel
ms.date: 02/26/2020
ms.topic: reference
ms.prod: microsoft-edge
ms.technology: webview
keywords: IWebView2, IWebView2WebView, webview2, WebView, aplicaciones Win32, Win32, Edge, ICoreWebView2, ICoreWebView2Host, control de explorador, HTML Edge
ms.openlocfilehash: 8fd3533d8f479866989f719be6e48c437fae4ddb
ms.sourcegitcommit: 07cda56425e5fdf90eeb3972e17041261bf720cd
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/14/2020
ms.locfileid: "10655421"
---
# <span data-ttu-id="bb846-104">interfaz ICoreWebView2HistoryChangedEventHandler</span><span class="sxs-lookup"><span data-stu-id="bb846-104">interface ICoreWebView2HistoryChangedEventHandler</span></span> 

> [!NOTE]
> <span data-ttu-id="bb846-105">Esta interfaz puede modificarse o no estar disponible para las versiones posteriores a la versión de SDK 0.9.430.</span><span class="sxs-lookup"><span data-stu-id="bb846-105">This interface may be altered or unavailable for releases after SDK version 0.9.430.</span></span> <span data-ttu-id="bb846-106">Consulta la [referencia](../../../webview2-api-reference.md) de la API más reciente.</span><span class="sxs-lookup"><span data-stu-id="bb846-106">Please refer to [Reference](../../../webview2-api-reference.md) for the latest API reference.</span></span>

```
interface ICoreWebView2HistoryChangedEventHandler
  : public IUnknown
```

<span data-ttu-id="bb846-107">La persona que llama implementa esta interfaz para recibir el evento HistoryChanged.</span><span class="sxs-lookup"><span data-stu-id="bb846-107">The caller implements this interface to receive the HistoryChanged event.</span></span>

## <span data-ttu-id="bb846-108">Resumen</span><span class="sxs-lookup"><span data-stu-id="bb846-108">Summary</span></span>

 <span data-ttu-id="bb846-109">Miembros</span><span class="sxs-lookup"><span data-stu-id="bb846-109">Members</span></span>                        | <span data-ttu-id="bb846-110">Descripciones</span><span class="sxs-lookup"><span data-stu-id="bb846-110">Descriptions</span></span>
--------------------------------|---------------------------------------------
[<span data-ttu-id="bb846-111">Invoke</span><span class="sxs-lookup"><span data-stu-id="bb846-111">Invoke</span></span>](#invoke) | <span data-ttu-id="bb846-112">No hay argumentos de evento y el parámetro args será null.</span><span class="sxs-lookup"><span data-stu-id="bb846-112">There are no event args and the args parameter will be null.</span></span>

## <span data-ttu-id="bb846-113">Miembros</span><span class="sxs-lookup"><span data-stu-id="bb846-113">Members</span></span>

#### <span data-ttu-id="bb846-114">Invoke</span><span class="sxs-lookup"><span data-stu-id="bb846-114">Invoke</span></span> 

<span data-ttu-id="bb846-115">No hay argumentos de evento y el parámetro args será null.</span><span class="sxs-lookup"><span data-stu-id="bb846-115">There are no event args and the args parameter will be null.</span></span>

> <span data-ttu-id="bb846-116">invocación [Invoke](#invoke)pública de HRESULT ([ICoreWebView2](ICoreWebView2.md) \* WebView, IUnknown \* args)</span><span class="sxs-lookup"><span data-stu-id="bb846-116">public HRESULT [Invoke](#invoke)([ICoreWebView2](ICoreWebView2.md) \* webview,IUnknown \* args)</span></span>
