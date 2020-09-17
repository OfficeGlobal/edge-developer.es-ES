---
description: Insertar tecnologías web (HTML, CSS y JavaScript) en las aplicaciones nativas con el control Microsoft Edge WebView2
title: WebView2 Win32 C++ ICoreWebView2ContainsFullScreenElementChangedEventHandler
author: MSEdgeTeam
ms.author: msedgedevrel
ms.date: 09/09/2020
ms.topic: reference
ms.prod: microsoft-edge
ms.technology: webview
keywords: IWebView2, IWebView2WebView, webview2, WebView, aplicaciones Win32, Win32, Edge, ICoreWebView2, ICoreWebView2Controller, control de explorador, HTML Edge, ICoreWebView2ContainsFullScreenElementChangedEventHandler
ms.openlocfilehash: 0477f9868dc472cab71dad4b10ff85fa034515a1
ms.sourcegitcommit: 0faf538d5033508af4320b9b89c4ed99872f0574
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/10/2020
ms.locfileid: "11012774"
---
# <span data-ttu-id="20147-104">interfaz ICoreWebView2ContainsFullScreenElementChangedEventHandler</span><span class="sxs-lookup"><span data-stu-id="20147-104">interface ICoreWebView2ContainsFullScreenElementChangedEventHandler</span></span> 

```
interface ICoreWebView2ContainsFullScreenElementChangedEventHandler
  : public IUnknown
```

<span data-ttu-id="20147-105">La persona que llama implementa este método para recibir los eventos ContainsFullScreenElementChanged.</span><span class="sxs-lookup"><span data-stu-id="20147-105">The caller implements this method to receive the ContainsFullScreenElementChanged events.</span></span>

## <span data-ttu-id="20147-106">Resumen</span><span class="sxs-lookup"><span data-stu-id="20147-106">Summary</span></span>

 <span data-ttu-id="20147-107">Miembros</span><span class="sxs-lookup"><span data-stu-id="20147-107">Members</span></span>                        | <span data-ttu-id="20147-108">Descripciones</span><span class="sxs-lookup"><span data-stu-id="20147-108">Descriptions</span></span>
--------------------------------|---------------------------------------------
[<span data-ttu-id="20147-109">Invoke</span><span class="sxs-lookup"><span data-stu-id="20147-109">Invoke</span></span>](#invoke) | <span data-ttu-id="20147-110">Se llama para proporcionar al implementador los argumentos del evento para el evento correspondiente.</span><span class="sxs-lookup"><span data-stu-id="20147-110">Called to provide the implementer with the event args for the corresponding event.</span></span>

<span data-ttu-id="20147-111">No hay argumentos de evento para este evento.</span><span class="sxs-lookup"><span data-stu-id="20147-111">There are no event args for this event.</span></span>

## <span data-ttu-id="20147-112">Miembros</span><span class="sxs-lookup"><span data-stu-id="20147-112">Members</span></span>

#### <span data-ttu-id="20147-113">Invoke</span><span class="sxs-lookup"><span data-stu-id="20147-113">Invoke</span></span> 

<span data-ttu-id="20147-114">Se llama para proporcionar al implementador los argumentos del evento para el evento correspondiente.</span><span class="sxs-lookup"><span data-stu-id="20147-114">Called to provide the implementer with the event args for the corresponding event.</span></span>

> <span data-ttu-id="20147-115">invocación [Invoke](#invoke)pública de HRESULT ([ICoreWebView2](icorewebview2.md) \* Sender, IUnknown \* args)</span><span class="sxs-lookup"><span data-stu-id="20147-115">public HRESULT [Invoke](#invoke)([ICoreWebView2](icorewebview2.md) \* sender, IUnknown \* args)</span></span>

<span data-ttu-id="20147-116">No hay argumentos de evento y el parámetro args será null.</span><span class="sxs-lookup"><span data-stu-id="20147-116">There are no event args and the args parameter will be null.</span></span>
