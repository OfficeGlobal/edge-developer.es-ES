---
description: Hospedar contenido web en la aplicación Win32 con el control Microsoft Edge WebView2
title: Microsoft Edge WebView2 para aplicaciones Win32
author: MSEdgeTeam
ms.author: msedgedevrel
ms.date: 12/09/2019
ms.topic: reference
ms.prod: microsoft-edge
ms.technology: webview
keywords: IWebView2, IWebView2WebView, webview2, WebView, aplicaciones Win32, Win32, Edge
ms.openlocfilehash: 23cce166d4ef2d05b6ffe5814c1568f75a72be0e
ms.sourcegitcommit: 07cda56425e5fdf90eeb3972e17041261bf720cd
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/14/2020
ms.locfileid: "10655145"
---
# <span data-ttu-id="59423-104">interfaz IWebView2FocusChangedEventHandler</span><span class="sxs-lookup"><span data-stu-id="59423-104">interface IWebView2FocusChangedEventHandler</span></span> 

> [!NOTE]
> <span data-ttu-id="59423-105">Esta interfaz puede modificarse o no estar disponible para las versiones posteriores a la versión de SDK 0.8.355.</span><span class="sxs-lookup"><span data-stu-id="59423-105">This interface may be altered or unavailable for releases after SDK version 0.8.355.</span></span> <span data-ttu-id="59423-106">Consulta la [referencia](../../../webview2-api-reference.md) de la API más reciente.</span><span class="sxs-lookup"><span data-stu-id="59423-106">Please refer to [Reference](../../../webview2-api-reference.md) for the latest API reference.</span></span>

```
interface IWebView2FocusChangedEventHandler
  : public IUnknown
```

<span data-ttu-id="59423-107">La persona que llama implementa este método para recibir los eventos GotFocus y LostFocus.</span><span class="sxs-lookup"><span data-stu-id="59423-107">The caller implements this method to receive the GotFocus and LostFocus events.</span></span>

## <span data-ttu-id="59423-108">Resumen</span><span class="sxs-lookup"><span data-stu-id="59423-108">Summary</span></span>

 <span data-ttu-id="59423-109">Miembros</span><span class="sxs-lookup"><span data-stu-id="59423-109">Members</span></span>                        | <span data-ttu-id="59423-110">Descripciones</span><span class="sxs-lookup"><span data-stu-id="59423-110">Descriptions</span></span>
--------------------------------|---------------------------------------------
[<span data-ttu-id="59423-111">Invoke</span><span class="sxs-lookup"><span data-stu-id="59423-111">Invoke</span></span>](#invoke) | <span data-ttu-id="59423-112">Se llama para proporcionar al implementador los argumentos del evento para el evento correspondiente.</span><span class="sxs-lookup"><span data-stu-id="59423-112">Called to provide the implementer with the event args for the corresponding event.</span></span>

<span data-ttu-id="59423-113">No hay argumentos de evento para este evento.</span><span class="sxs-lookup"><span data-stu-id="59423-113">There are no event args for this event.</span></span>

## <span data-ttu-id="59423-114">Miembros</span><span class="sxs-lookup"><span data-stu-id="59423-114">Members</span></span>

#### <span data-ttu-id="59423-115">Invoke</span><span class="sxs-lookup"><span data-stu-id="59423-115">Invoke</span></span> 

<span data-ttu-id="59423-116">Se llama para proporcionar al implementador los argumentos del evento para el evento correspondiente.</span><span class="sxs-lookup"><span data-stu-id="59423-116">Called to provide the implementer with the event args for the corresponding event.</span></span>

> <span data-ttu-id="59423-117">invocación [Invoke](#invoke)pública de HRESULT ([IWebView2WebView](IWebView2WebView.md) \* WebView, IUnknown \* args)</span><span class="sxs-lookup"><span data-stu-id="59423-117">public HRESULT [Invoke](#invoke)([IWebView2WebView](IWebView2WebView.md) \* webview,IUnknown \* args)</span></span>

<span data-ttu-id="59423-118">No hay argumentos de evento y el parámetro args será null.</span><span class="sxs-lookup"><span data-stu-id="59423-118">There are no event args and the args parameter will be null.</span></span>
