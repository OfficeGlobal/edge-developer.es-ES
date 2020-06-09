---
description: Hospedar contenido web en la aplicación Win32 con el control Microsoft Edge WebView2
title: Microsoft Edge WebView2 para aplicaciones Win32
author: MSEdgeTeam
ms.author: msedgedevrel
ms.date: 06/05/2020
ms.topic: reference
ms.prod: microsoft-edge
ms.technology: webview
keywords: IWebView2, IWebView2WebView, webview2, WebView, aplicaciones Win32, Win32, Edge, ICoreWebView2, ICoreWebView2Controller, control de explorador, HTML Edge
ms.openlocfilehash: 8c717bb57a5dc984d6cb2bbbbac79cf91d64fe2f
ms.sourcegitcommit: 8dca1c1367853e45a0a975bc89b1818adb117bd4
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/08/2020
ms.locfileid: "10699379"
---
# <span data-ttu-id="fb576-104">interfaz ICoreWebView2ContainsFullScreenElementChangedEventHandler</span><span class="sxs-lookup"><span data-stu-id="fb576-104">interface ICoreWebView2ContainsFullScreenElementChangedEventHandler</span></span> 

```
interface ICoreWebView2ContainsFullScreenElementChangedEventHandler
  : public IUnknown
```

<span data-ttu-id="fb576-105">La persona que llama implementa este método para recibir los eventos ContainsFullScreenElementChanged.</span><span class="sxs-lookup"><span data-stu-id="fb576-105">The caller implements this method to receive the ContainsFullScreenElementChanged events.</span></span>

## <span data-ttu-id="fb576-106">Resumen</span><span class="sxs-lookup"><span data-stu-id="fb576-106">Summary</span></span>

 <span data-ttu-id="fb576-107">Miembros</span><span class="sxs-lookup"><span data-stu-id="fb576-107">Members</span></span>                        | <span data-ttu-id="fb576-108">Descripciones</span><span class="sxs-lookup"><span data-stu-id="fb576-108">Descriptions</span></span>
--------------------------------|---------------------------------------------
[<span data-ttu-id="fb576-109">Invoke</span><span class="sxs-lookup"><span data-stu-id="fb576-109">Invoke</span></span>](#invoke) | <span data-ttu-id="fb576-110">Se llama para proporcionar al implementador los argumentos del evento para el evento correspondiente.</span><span class="sxs-lookup"><span data-stu-id="fb576-110">Called to provide the implementer with the event args for the corresponding event.</span></span>

<span data-ttu-id="fb576-111">No hay argumentos de evento para este evento.</span><span class="sxs-lookup"><span data-stu-id="fb576-111">There are no event args for this event.</span></span>

## <span data-ttu-id="fb576-112">Miembros</span><span class="sxs-lookup"><span data-stu-id="fb576-112">Members</span></span>

#### <span data-ttu-id="fb576-113">Invoke</span><span class="sxs-lookup"><span data-stu-id="fb576-113">Invoke</span></span> 

<span data-ttu-id="fb576-114">Se llama para proporcionar al implementador los argumentos del evento para el evento correspondiente.</span><span class="sxs-lookup"><span data-stu-id="fb576-114">Called to provide the implementer with the event args for the corresponding event.</span></span>

> <span data-ttu-id="fb576-115">invocación [Invoke](#invoke)pública de HRESULT ([ICoreWebView2](icorewebview2.md) \* Sender, IUnknown \* args)</span><span class="sxs-lookup"><span data-stu-id="fb576-115">public HRESULT [Invoke](#invoke)([ICoreWebView2](icorewebview2.md) \* sender, IUnknown \* args)</span></span>

<span data-ttu-id="fb576-116">No hay argumentos de evento y el parámetro args será null.</span><span class="sxs-lookup"><span data-stu-id="fb576-116">There are no event args and the args parameter will be null.</span></span>
